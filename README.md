
    👋 Hi, I’m @mfahadahmed2020
    👀 I’m interested in ... Computing
    🌱 I’m currently learning ... OnLine Computing
    💞️ I’m looking to collaborate on ... Social Media SEO
    I am a Students ...
    I am not a Coding Developers, But I Have Worked on the Windows Installation, Configuration, and Windows Programming Development of all Windows Versions from Windows 98 to the latest. I Have Experience in Developing Corrupted Windows and Corrupted Programs Within Windows.
    Additionally, I Have Worked as an IT Advisor, Specializing in Troubleshooting Technical Issues and System Optimization.

Skills & Expertise

    Windows Installation & Configuration
    Corrupt Windows & Software Development
    IT Advisory & System Optimization
    Troubleshooting & Technical Support

Technologies & Tools
Windows
Development
IT Advisor
Troubleshooting
System Optimization
Networking
1. Install Each Version on FAT32 File System:

    Windows 95
    Windows 97
    Windows 98
    Windows 2000
    Windows Millennium
    Windows XP

2. Install Each Version on NTFS File System:

    Windows 2000

    Windows Millennium

    Windows XP

    Windows 7

    Windows 8

    Windows 9

    Windows 10

    Windows 11

    📫 How to reach me ...

    😄 Pronouns: ...

    ⚡ Fun fact: ...


💫 About Me:

🧠 Diving Deep InTo Agentic & Robotics AI System Learning

🎓 AS A Student At Governor House Sindh IT Marque GenAI, Web3 & Metaverse Initiative

🔗 Portfolio: M Fahad Ahmed Portfolio

🚀 Crafting Powerful Semi-Stack & AI-Driven Applications Using Next.js 15, Tailwind CSS, FastAPI, Streamlit, CrewAI & more

🤝 Passionate About Building Intelligent, Responsive, Web Applications, Or AI Agents

💬 Let’s Talk About Anything From Modern Web/App Development To GenAI, SDKs, OpenAI Agents & Metaverse Innovations

💻 Tech Stack:
    TypeScript JavaScript Python HTML5 CSS3 Next JS TailwindCSS BootStrap NodeJS FastAPI Streamlit Pydantic MongoDB
    OpenAI REST API Gemini Jupyter Notebook Chainlit Sanity CMS Stripe  Figma

📊 GitHub Status:



<img width="300" height="165" alt="image" src="https://github.com/user-attachments/assets/0247db80-0274-46fd-81de-c4fd09053454" />




<img width="495" height="195" alt="image" src="https://github.com/user-attachments/assets/acf02302-afdb-4f70-986f-67ce4ee627e7" />




📫 Let's Connect!

LinkedIn            FaceBook        Xx            Gmail            YouTube

<img width="57" height="20" alt="image" src="https://github.com/user-attachments/assets/afc249fd-10a8-4807-9669-6aefaa5e72cf" />https://www.linkedin.com/in/m-ahmed-111b3b203/

https://www.facebook.com/mfahad.ahmed.5?mibextid=ZbWKwL

<img width="35" height="20" alt="image" src="https://github.com/user-attachments/assets/bdeb3a3c-0b9e-4418-aaee-88539ba81692" />https://x.com/MFahadAhmed4?t=6ek1JzhBpRtJTaBsGaoi4g&s=08

<img width="59" height="20" alt="image" src="https://github.com/user-attachments/assets/322de864-dcf2-42cd-a1b5-c435b70d1623" />https://www.mfahadahmed2020@gmail.com

https://youtube.com/@Walmartfashionaccessories?si=lLb7DFzSAQmEkPck









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

          
<img width="880" height="206" alt="image" src="https://github.com/user-attachments/assets/effa0554-6925-4ef5-9e62-0ce9bed9b83f" />


<img width="880" height="192" alt="image" src="https://github.com/user-attachments/assets/bfb6c8cf-4c37-43ca-a2ee-23b8d6fa4f4b" />



