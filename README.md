<!-- PROJECT LOGO -->
<br />
<div align="center">
    <img src="https://github.com/Pramit726/CompreHive/assets/149934842/da9d2975-76c8-4a3f-ac06-4984bc100d82" alt="Logo" width="80" height="80">
  </a>
  <h3 align="center">CompreHive</h3>

  <p align="center">
    Enhance understanding effortlessly with customized reading passages and questions
    <br />
    <a href="https://github.com/Pramit726/CompreHive/assets/149934842/43ef4642-55e9-4be0-9dff-14684bee0c43">View Demo</a>
    ·
    <a href="">Report Bug</a>
    ·
    <a href="">Request Feature</a>
  </p>
</div>


## Project Overview

<div align="justify"> 
This Streamlit application, powered by Google GEMINI 1.5 Pro, generates comprehension exercises based on user input of topics, keywords, and desired question types. Users have the flexibility to specify the number of multiple-choice, short-answer, and long-answer questions according to their preferences. Moreover, users can conveniently download the generated content in the form of text and PDF files, enhancing accessibility and offline usage.
</div>
</br>

<div align="justify"> 
The application incorporates robust logging and exception handling mechanisms to ensure smooth operation and error detection. Additionally, a setup module is implemented to streamline the installation process and manage dependencies effectively.
</div>
</br>

<div align="justify"> 
Deployed on Amazon Web Services (AWS), the application offers easy access and utilization for users. AWS also ensures scalability, allowing the application to handle varying user loads seamlessly. 
</div>


## Project Demo

- **App Recording**

https://github.com/Pramit726/CompreHive/assets/149934842/5dea4867-17dd-4d1f-842b-1767732834a4

<br/>

- **Text File Screenshot**

<!-- ![App Screenshot](https://github.com/Pramit726/CompreHive/assets/149934842/8acc6b76-40f8-4137-9b74-9413ea2af5de) --> 
<img src="https://github.com/Pramit726/CompreHive/assets/149934842/8acc6b76-40f8-4137-9b74-9413ea2af5de" alt="Text-screenshot" width="500" height="700">

<br/>
<br/>

- **PDF File Screenshot**

<!-- ![App Screenshot](https://github.com/Pramit726/CompreHive/assets/149934842/fa5c1253-155c-4dbb-b499-032628fe7cab)--> 
<img src="https://github.com/Pramit726/CompreHive/assets/149934842/fa5c1253-155c-4dbb-b499-032628fe7cab" alt="PDF-screenshot" width="500" height="874">

## Required API Keys

This project requires two API keys:

- **Google API key:** Required for accessing the GEMINI 1.5 Pro model.
- **LangChain API key:** Required for LangSmith tracking.

Ensure that you obtain these API keys before running the project.

## Project Setup

**Clone this GitHub repository**

```bash
  (base)$: git clone https://github.com/Pramit726/CompreHive.git
```

**Go to the project directory**

```bash
  (base)$: cd CompreHive
```

**Configure environment**

- Create the conda environment

```bash
(base)$: conda  create -p venv python==3.10 -y
```

- Activate the environment

```bash
(base)$: conda activate venv
```
- Install the required dependencies

```bash
(venv)$: pip install -r requirements.txt
```
**Run it**

```bash
(venv)$: streamlit run app.py
```

As soon as you run the script, a local Streamlit server will spin up, and your app will open in a new tab in your default web browser.

Or you can navigate to ``http://localhost:8501.``

## Deployment on AWS

**Step 1**

First login to the AWS: https://aws.amazon.com/console/

**Step 2**

Search about EC2 in the services section.

**Step 3**

Configure the Ubuntu machine.

**Step 4**

Launch the instance.

**Step 5**

Do the port mapping to this port: 8501

**Step 6**

Run the following commands

```bash
sudo apt update
```

```bash
sudo apt-get update
```
```bash
sudo apt upgrade -y
```
```bash
sudo apt install git curl unzip tar make sudo vim wget -y
```
```bash
git clone https://github.com/Pramit726/CompreHive.git
```

```bash
cd CompreHive
```

```bash
sudo apt install python3-pip
```

```bash
sudo apt install python3-venv
```

```bash
python3 -m venv venv
```

```bash
source venv/bin/activate
```

```bash
pip3 install -r requirements.txt
```

**If you want to add the API keys**

- Create .env file in the AWS server using  touch .env.

- Next write vi .env

- Press i 

- Copy API keys and paste it

- Press : , then wq! and hit enter

**Step 7**
```bash
#Temporary running
python3 -m streamlit run app.py
```

```bash
#Permanent running
nohup python3 -m streamlit run app.py
```

## Dependencies

- langchain-core
- langchain-google-genai
- python-dotenv
- reportlab
- streamlit

## Author

 **[Pramit De](https://github.com/Pramit726)**  
 - pramitde726@gmail.com / pramit.de.cse.2021@tint.edu.in 

- Department of CSE, Techno International New Town, West Bengal, India 
© 2024 CompreHive by Pramit De 








