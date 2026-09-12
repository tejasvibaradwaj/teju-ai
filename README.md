      - name: Extract Android project
        run: |
          unzip -o *.zip
          PROJECT_DIR=$(find . -maxdepth 2 -name settings.gradle.kts -printf '%h\n' | head -1)
          echo "PROJECT_DIR=$PROJECT_DIR" >> $GITHUB_ENV# teju-ai
