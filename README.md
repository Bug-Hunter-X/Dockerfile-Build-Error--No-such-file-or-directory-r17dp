# Dockerfile Bug: Missing requirements.txt

This repository demonstrates a common error when building Docker images: a missing or incorrectly referenced requirements.txt file.  The original Dockerfile attempts to install Python packages using `pip3 install -r requirements.txt`, but the file is missing, resulting in a build failure.

The solution demonstrates the corrected Dockerfile, ensuring the `requirements.txt` file is present and correctly referenced.

**Bug:** The original Dockerfile fails to build because the `requirements.txt` file, necessary for installing Python dependencies, is not included in the image or is in the wrong location.

**Solution:** The corrected Dockerfile includes the `requirements.txt` file and verifies the correct path to the file.