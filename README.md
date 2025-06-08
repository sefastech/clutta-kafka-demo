# Clutta-Kafka Codespaces Demo

Welcome! This repository provides a quick and easy way to experience Clutta using GitHub Codespaces. Follow these steps to get a live demo of your Kafka flows being monitored.

## Get Started in 5 Easy Steps

### Step 1: Set Up Your Project on Our UI

Before you work with Codespaces, you'll need to create a project on our platform first.

1.  **Sign Up & Create a Project:**
    * Visit our UI at [Clutta](https://dev.clutta.io/).
    * Sign up for an account (if you haven't already).
    * Create a new project. During this process, you'll select your preferred Kafka flows that you want to observe.

2.  **Copy Your Agent Configuration:**
    * After creating your project, you'll be directed to the **Provisioning Screen**.
    * You'll see 2 steps listed. Your focus is on the second one for this demo.
    * Beside step 2 which is titled: **Update environment variables**, you'll see a YAML configuration file. **Copy the entire content of this YAML file.** You'll need it shortly.

    *(Note: The first step on the provisioning screen involves adding our agent to your `docker-compose.yaml`. For this demo, we've already handled that for you!)*

---

### Step 2: Launch Your Codespace

Now, let's get your demo environment ready!

1.  **Open this GitHub Repository:**
    * Navigate back to this GitHub repository: [Clutta-Kafka Demo Repository](https://github.com/sefastech/clutta-kafka-demo/)

2.  **Create a Codespace:**
    * Click on the `<> Code` button.
    * Select the `Codespaces` tab.
    * Click `Create codespace on main`.
    * **Important:** Ensure the machine type selected is **4-core** for optimal performance.

---

### Step 3: Paste Your Configuration

Once your Codespace is open, it's time to add your specific project configuration.

1.  **Locate `clutta-agent-config.yaml`:**
    * In the Codespace file explorer (left sidebar), find and open the file named `clutta-agent-config.yaml`.

2.  **Paste Your YAML:**
    * Delete any existing content in `clutta-agent-config.yaml`.
    * Paste the YAML configuration you copied from our UI (in Step 1.2) into this file.

---

### Step 4: Run the Demo Environment

Almost there! Let's bring everything online.

1.  **Open the Terminal:**
    * If the terminal isn't already open, go to `Terminal > New Terminal` in the Codespace menu.

2.  **Start Docker Compose:**
    * In the terminal, run the following command:

        ```bash
        docker compose up -d
        ```
    * This will start all the necessary services in the background. Please wait for the command to complete.

---

### Step 5: See Your Observability in Action!

Once `docker compose up -d` has finished running in your Codespaces terminal, **switch back to the browser tab where Clutta UI is open.**

1.  **Check for Redirection:**
    * You should now see that your UI has **automatically redirected** you from the provisioning screen to your **Project Screen**.

2.  **View Your Pulses:**
    * On the Project Screen, you'll find a table displaying pulses, which are live data from your Kafka flows, demonstrating our product's observability capabilities!

---

Enjoy your demo! If you have any questions or encounter issues, please contact our support team.
