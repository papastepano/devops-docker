# Step 1: Clone the repository without checking out files

    git clone --no-checkout https://github.com/docker-hy/material-applications.git repo

## Step 2: Change directory to the local repository

cd repo

## Step 3: Enable sparse-checkout

git sparse-checkout init --cone

## Step 4: Specify the folder to check out

git sparse-checkout set example-frontend

## Step 5: Check out the branch

git checkout main
