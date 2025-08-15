- 👋 Hi, I’m @mfahadahmed2020
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- I am a Students ...
- I am not a Coding Developers, But I Have Worked on the Windows Installation, Configuration, and Windows Programming Development of all Windows Versions from Windows 98 to the latest. I Have Experience in Developing Corrupted Windows and Corrupted Programs Within Windows.  
Additionally, I Have Worked as an IT Advisor, Specializing in Troubleshooting Technical Issues and System Optimization.  

## Skills & Expertise

- Windows Installation & Configuration  
- Corrupt Windows & Software Development  
- IT Advisory & System Optimization  
- Troubleshooting & Technical Support  

## Technologies & Tools

# Windows
# Development
# IT Advisor
# Troubleshooting
# System Optimization
# Networking

# 1. Install Each Version on FAT32 File System:

   - Windows 95
   - Windows 97
   - Windows 98
   - Windows 2000
   - Windows Millennium
   - Windows XP

# 2. Install Each Version on NTFS File System:

   - Windows 2000
   - Windows Millennium
   - Windows XP
   - Windows 7
   - Windows 8
   - Windows 9
   - Windows 10
   - Windows 11

   - 📫 How to reach me ...
   - 😄 Pronouns: ...
   - ⚡ Fun fact: ...

name: GitHub Snake Game



on:

  # Schedule the workflow to run daily at midnight UTC

  schedule:

    - cron: "0 0 * * *"



  # Allow manual triggering of the workflow

  workflow_dispatch:



  # Trigger the workflow on pushes to the main branch

  push:

    branches:

      - main



jobs:

  generate:

    runs-on: ubuntu-latest

    timeout-minutes: 10



    steps:

      # Step 1: Checkout the repository

      - name: Checkout Repository

        uses: actions/checkout@v3



      # Step 2: Generate the snake animations

      - name: Generate GitHub Contributions Snake Animations

        uses: Platane/snk@v3

        with:

          # GitHub username to generate the animation for

          github_user_name: ${{ github.repository_owner }}



          # Define the output files and their configurations

          outputs: |

            dist/github-snake.svg

            dist/github-snake-dark.svg?palette=github-dark

            dist/ocean.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9

        env:

          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}



      # Step 3: Deploy the generated files to the 'output' branch

      - name: Deploy to Output Branch

        uses: peaceiris/actions-gh-pages@v3

        with:

          github_token: ${{ secrets.GITHUB_TOKEN }}

          publish_dir: ./dist

          publish_branch: output

          # Optionally, you can set a custom commit message

          commit_message: "Update snake animation [skip ci]"
