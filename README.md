<!DOCTYPE html>
<html>
<head>
    <title>GitDemo - README</title>
    <meta charset="UTF-8">
</head>
<body style="font-family: Arial, sans-serif; line-height: 1.6;">

<h1>GitDemo</h1>
<p><strong>Author:</strong> Saptarshi Jana</p>

<hr>

<h2>1. Introduction</h2>
<p>This repository contains basic Git commands and workflow examples for beginners using Git Bash and PowerShell.</p>

<hr>

<h2>2. Git Installation & Initial Configuration</h2>
<p>After installing <strong>Git Bash</strong>, configure your identity:</p>

<pre>
git config --global user.name "SaptarshiJana07"
git config --global user.email "mesaptarshi.jana@gmail.com"
git config --list
</pre>

<hr>

<h2>3. Viewing Files in Local Repository</h2>

<p><strong>PowerShell Commands:</strong></p>
<ul>
    <li>View all files: <code>Get-ChildItem -Force</code></li>
    <li>View only hidden files: <code>Get-ChildItem -Force -Hidden</code></li>
</ul>

<p><strong>Git Bash command to show files:</strong></p>
<pre>ls [-Attributes | -Directory | -File | -Hidden | -ReadOnly | -System]</pre>

<p><strong>Initialize Git in a folder:</strong></p>
<pre>git init</pre>

<p><strong>Clone a remote GitHub repository:</strong></p>
<pre>git clone https://github.com/SaptarshiJana07/GitDemo.git</pre>

<hr>

<h2>4. Git Workflow (Local to Remote)</h2>

<ol>
    <li>Create a GitHub repository</li>
    <li>Clone it into your local folder:
        <pre>git clone https://github.com/SaptarshiJana07/GitDemo.git</pre>
    </li>
    <li>Make changes to files</li>
    <li>Stage changes:
        <pre>git add .</pre>
    </li>
    <li>Commit changes:
        <pre>git commit -m "message"</pre>
    </li>
    <li>Push to GitHub:
        <pre>git push -u origin main</pre>
    </li>
    <li>Pull updates from remote (if changed online):
        <pre>git pull origin main</pre>
    </li>
</ol>

<p><strong>Check remote repository:</strong></p>
<pre>git remote -v</pre>

<hr>

<h2>5. Checking File Status</h2>

<p>Use:</p>
<pre>git status</pre>

<p><strong>Possible File States:</strong></p>
<ul>
    <li>Untracked</li>
    <li>Modified</li>
    <li>Staged</li>
    <li>Unmodified</li>
</ul>

<p><strong>Typical Outputs:</strong></p>
<pre>
On branch main
Your branch is up to date with 'origin/main'.
Nothing to commit, working tree clean
</pre>

<p>Or:</p>
<pre>
On branch main
Changes not staged for commit:
    modified: README.md
</pre>

<p><strong>Solutions:</strong></p>
<ul>
    <li>Stage changes: <code>git add &lt;file&gt;</code></li>
    <li>Discard changes: <code>git restore &lt;file&gt;</code></li>
    <li>Commit tracked changes: <code>git commit -a -m "message"</code></li>
</ul>

<hr>

<h2>6. Staging & Saving Changes</h2>

<p><strong>Stage all changes:</strong></p>
<pre>git add .</pre>

<p><strong>Commit to local repository:</strong></p>
<pre>git commit -m "new file added"</pre>

<hr>

<h2>7. Pushing to GitHub</h2>

<p><strong>Push to main branch:</strong></p>
<pre>git push origin main</pre>

<p><strong>Push to another branch (e.g., branch1):</strong></p>
<pre>git push origin branch1</pre>

<hr>

<h2>8. Working with Branches</h2>

<ul>
    <li>List branches:
        <pre>git branch</pre>
    </li>

    <li>Create a new branch:
        <pre>git branch [branch-name]</pre>
    </li>

    <li>Create and switch to a new branch:
        <pre>git checkout -b person1</pre>
    </li>

    <li>Switch to existing branch:
        <pre>git checkout [branch-name]</pre>
    </li>

    <li>Merge a branch into the current branch:
        <pre>git merge [branch]</pre>
    </li>

    <li>Delete a branch (after switching away from it):
        <pre>git branch -d person1</pre>
    </li>

    <li>View commit history:
        <pre>git log</pre>
    </li>
</ul>

<hr>

<h2>9. Summary</h2>
<p>This README provides a simplified and structured guide to Git basics, including configuration, workflow, status checking, branching, and pushing/pulling updates. It is ideal for beginners using Git Bash or PowerShell.</p>

</body>
</html>
