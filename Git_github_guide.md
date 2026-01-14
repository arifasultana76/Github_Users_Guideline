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