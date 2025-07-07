<p align="center">
  <img width="250px" src="./images/cover.png">
</p>
<h1 align="center">Contributor</h1>

This repository automates contributions to your GitHub contribution graph by incrementing a counter and committing changes.

---

Result:
<p align="center">
  <img width="" src="./images/you.jpeg">
</p>

## How It Works

The workflow updates the `contrib.txt` file with an incremented value each time it runs, effectively filling up your contribution graph.

---

## Setup Instructions

### 1. **Fork and Clone**

- Fork this repository to your GitHub account.
- Clone the forked repository:

   ```bash
   git clone <your-fork-url>
   cd contributor
   ```

### 2. **Configure GitHub Actions**

Ensure the workflow file (`contrib.yml`) is set up under `.github/workflows/`.

### 3. **Add Secrets**

Add the following secrets in your repository settings:

- `GH_EMAIL` – Your GitHub email address.
- `GH_USERNAME` – Your GitHub username.

### 4. **Enable Workflow Permissions**

Allow the workflow to commit changes:

- Go to **Settings** > **Actions** > **General** > **Workflow permissions**.
- Enable "Read and write permissions".
![](./images/perm.png)

---

## Running the Workflow

### **Manual Trigger (not recommented)**

- Go to the **Actions** tab.
- Select the "Contribute" workflow.
- Click **Run workflow**.

### **Scheduled Runs**

The workflow runs automatically every hour (`cron: '0 */1 * * *'`).

---

## License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.
