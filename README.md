# issf_world_rankings

## About the Project

This project is a scraper that captures [ISSF World Rankings](https://www.issf-sports.org/competitions/worldranking/complete_ranking_by_event_yearly.ashx) running on a scheduled job using GitHub Actions.

For more information on the process of creating this project, check out [this blog post](https://michaelwknott.github.io/issf-world-rankings-scraper-using-github-actions.html).

## Built With

+ [Python](https://www.python.org/)
+ [GitHub Actions](https://docs.github.com/actions)

## Getting Started

### Prerequisites

+ GitHub account

### Installation

To get a local copy up and running, follow these simple steps.

1. Clone the repo
    ```bash
    git clone git@github.com:michaelwknott/issf_world_rankings.git
    ```

2. Create a [GitHub repository](https://docs.github.com/en/get-started/quickstart/create-a-repo)
    
3. Link your local version to the GitHub repository
    ```bash
    git remote add origin git@github.com:<GITHUB_USERNAME>/<REPO_NAME>.git
    ```
    Ensure you change <GITHUB_USERNAME> and <REPO_NAME> to your GitHub username and repository name respectively.

4. Check the remote repository is set up correctly
    ```bash
    git remote -v
    ```
    You should see the something similar to the following:
    ```
    origin  git@github.com:<GITHUB_USERNAME>/<REPO_NAME>.git (fetch)
    origin  git@github.com:<GITHUB_USERNAME>/<REPO_NAME>.git (push)
    ```

5. Push to GitHub
    ```bash
     git push origin main
     ```

6. Run the GitHub Action manually to check it works
    + Go to the Actions tab in your repository
    + Click on the `Schedule ISSF Scraper` workflow
    + Click `Run workflow` in the top right corner
    + Click `Run workflow` in the pop-up window

7. Check the GitHub Action ran successfully
    + Go to the Actions tab in your repository
    + Click on the `Schedule ISSF Scraper` workflow
    + Click on the latest run of `Schedule ISSF Scraper`
    + Click on the `scrap_data` job
    + Check individual steps ran successfully

## License

Distributed under the MIT License. See LICENSE for more information.
