📘 Github Notes:

🔹 Branch সংক্রান্ত:

এখন কোন branch-এ আছো তা জানতে -> git branch

নতুন branch তৈরি + switch -> git checkout -b branch_name

Branch delete করার নিয়মঃ

-> যে branch ডিলিট করবে, সেটাতে থাকা যাবে না
-> git checkout main
-> git branch -d branch_name

🔹 Basic Git Workflow:

-> git add .
-> git commit -m "commit message"
-> git push origin branch_name

🔹 Open-source Contribution ধাপসমূহ:

-> অন্য কারো GitHub repository খুঁজে নাও
-> Repository fork করো
-> Fork করা repo clone করো
-> VS Code খুলে নতুন branch তৈরি করো
-> নতুন feature যোগ করো বা ফাইল আপডেট করো

Existing file আপডেট করলে:

-> git commit -am "message"

Branch push:

-> git push origin branch_name

GitHub-এ গিয়ে Pull Request (PR) করা:

sub-branch থেকে main branch-এ কোড আনার জন্য PR ব্যবহার হয়।

🔹 Pull Request & Merge

-> Compare & Pull Request বাটনে ক্লিক করো
-> Repo owner notification পাবে
-> Approve হলে কোড merge হবে

🔹 Git Conflict

-> একই ফাইল একই সময়ে আমি ও অন্য contributor
পরিবর্তন করলে git conflict হয়।

🔹 For check commit history:

-> git log
-> git log --oneline

🔹 git log

👉 এখন পর্যন্ত করা সব commit-এর বিস্তারিত ইতিহাস দেখায়

এতে দেখা যায়:

1. commit ID
2. কে commit করেছে
3. তারিখ
4. commit message

মানে: পুরো history (details সহ)

🔹 git log --oneline

👉 একই commit history এক লাইনে, ছোট করে দেখায়

এতে থাকে:

1. short commit ID
2. commit message

মানে: quick list / short view

👉 details চাইলে → git log
👉 দ্রুত দেখতে চাইলে → git log --oneline

পুরোনো commit-এ ফিরে যাওয়া (local):

-> git reset commit_id --hard

শেষ commit edit করা:

-> git commit --amend
-> git push --force

# PR পাঠানোর স্টেপ:

1️⃣ GitHub repo fork করো

যে project-এ contribute করতে চাও

Fork বাটনে ক্লিক করো
👉 নিজের GitHub-এ copy হবে

2️⃣ Repo clone করো (local PC তে)
git clone https://github.com/your-username/repo-name.git

3️⃣ Repo folder-এ ঢুকো
cd repo-name

4️⃣ New branch বানাও
git checkout -b fix-bug

5️⃣ Code change করো

Bug fix / feature / doc edit

File save করো

6️⃣ Change check করো
git status

7️⃣ Add & commit করো
git add .
git commit -m "Fix: small bug in login page"

8️⃣ GitHub-এ push করো
git push origin fix-bug

9️⃣ Pull Request খুলে ফেলো

GitHub repo-তে গেলে Compare & pull request দেখাবে

Click করো

Title + description লেখো

Create pull request

🔟 Review এর অপেক্ষা

Maintainer review করবে

Change চাইলে ঠিক করে আবার push করো

# Only repo clone:

1. Go to the repo which is you want to open your vs code.
2. Then click code then copy the repo url.
3. Create a folder for repo.
4. Then open created folder from your vs code. 
5. Next open new terminal
6. Then write --> git clone https://github.com/your-username/repo-name.git 
[ Here's just paste that copy url]
