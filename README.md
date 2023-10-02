# Cloud Computing Foundations

#### by Duke University

## Learning goals

- Learn how to build continuous delivery pipelines.
- Learn about the different types of Cloud service models.
- Learn how to utilize Infrastructure as Code to manage Cloud Infrastructure.
- Put theory into practice by doing the project.

Open the [notes from course =>](./notes.ipynb)

## Projects

### Scaffold

[![Test build Scaffold](https://github.com/agne6ka/duke-cloud-computing/actions/workflows/scaffold.yml/badge.svg)](https://github.com/agne6ka/duke-cloud-computing/actions/workflows/scaffold.yml)

1. Go to scaffold directory

    ```bash
    cd scaffold
    ```

2. Create Python virtual environment

    ```bash
    python3 -m venv ~/.scaffold
    ```

3. Activate the venv

    ```bash
    source ~/.scaffold/bin/activate
    ```

4. Install required packages

    ```bash
    make install
    ```

    Useful commands

    ```bash
    make all # install run test at once
    deactivate # exit the venv
    ```

### Hugo App

![Build with CodeBuild](https://codebuild.eu-north-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiaW1VVk1UZHJaWnFtaEhYVkh6dmlDajBneU56cDJGeXVFejFHSVA1ZXh6Vm5vMmF3dWZpTzh2ekZTNVNnakJEcFA1YTZvaUdrMURXcXhiK1ZIZEFxcFRRPSIsIml2UGFyYW1ldGVyU3BlYyI6IjA1UlRWV2tMTnFBd3ZJcm4iLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main)

1. Go to hugo-app

    ```bash
    cd hugo-app
    ```

2. Download hugo with compressed binary

    ```bash
    wget https://github.com/gohugoio/hugo/releases/download/v0.119.0/hugo_0.119.0_Linux-64bit.tar.gz
    # wget https://github.com/gohugoio/hugo/releases/download/v0.119.0/hugo_0.119.0_linux-arm64.tar.gz # AArch64
    ```

3. Uncompress the file

    ```bash
    tar zxvf hugo_0.119.0_Linux-64bit.tar.gz
    ```

4. Create `/bin` path if not exists

    ```bash
    mkdir -p ~/bin
    ```

5. Move the binary file to `bin` folder

    ```bash
    mv hugo ~/bin/
    ```

6. Build public files

    ```bash
    hugo
    ```

7. Serve hugo app

    ```bash
    hugo serve
    ```
