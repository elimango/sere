### sere ・/sir/ 
### *noun* 
a natural succession of plant communities, especially a full series from uncolonized habitat to the appropriate climax vegetation.  
<sub>*from<a href="https://languages.oup.com/google-dictionary-en/"> Oxford Languages and Google*,</a> (oed.com)</sub>

<hr></hr>

![image](https://github.com/user-attachments/assets/8b9b34e9-883f-4ad7-bf14-5f8996769369)

<hr></hr>

*Sere* is a lightweight gui wrapper for git, git servers (ex. GitHub, GitLab); using Git LFS, built strictly to propagate self-hosted production pipelines.

### Full Usage
<u>__Sere__</u> is primarily developed for *elimango/studio* (development lead by elimango), which is project managed using <a href="https://obsidian.md/">*Obsidian*</a>, a markdown based text editor that lives exclusively on your local device. Sere listens and shares git porcelain status with structures in your obsidian vault.

<u>__Sere__</u> is made feasible by the existence of <a href="https://github.com/git-lfs/git-lfs">*Git LFS (Large File Storage)*</a>
<blockquote>Git Large File Storage (LFS) replaces large files such as audio samples, videos, datasets, and graphics with text pointers inside Git, while storing the file contents on a remote server like GitHub.com or GitHub Enterprise.</blockquote>

*From Git LFS, https://git-lfs.com/*


## What does it do?
### Standalone
<ul>
  <li><a>Automatic commit versioning capabilities using a toggleable listening service in your repos to detect and push new file changes.</a></li>
  <li><a>Weighted automatic rebase to delete all but the most important versions of your projects and clean commit history to avoid large remote sizes.</a></li>
  <ul>
    <li><a>Sere will use min/max time scopes, <i>i.e '5 months.'</i> to determine if any commits made within that period are 'important'</a></li>
    <li><a>Sere will stage all commits outside of this time scope as wilted, and will prompt if they are safe to be excluded from the rebase (deleted).</a></li>
    <li><a>Additionally, users can set a maximum number of commits from the latest commit to exist at a time, and perform an automatic rebase each time it is exceeded.</a></li>    
  </ul>
  
  <li><a>'Flowerbeds' or, 'Beds', for short.</a></li>
  <ul>
    <li><a>A '.gitignore' scope that allows passthrough of individual files for sequence file management. (ex. render passes)</a></li>
    <li><a>When beds check local against remote for files of a sequence in a directory, they will <b><i>not</i></b> pull all files into the staging area, local users will have full control over which files and how many they wish to check out from remote. </a></li>
  </ul>
  <li><a>Stores configuration and installation information in a json format for automatic updates and setup migration.</a></li> 
</ul>
  
### Obsidian Integration
<ul>
  <li><a>Downloads and installs obsidian directly from git releases if the user is missing an installation.</a></li>  
  <li><a>Downloads and initializes obsidian vaults from a remote repo, with api token handling. See <b><i><a href="https://github.com/Vinzent03/obsidian-git">Obsidian Git </a></i></b>for more about this workflow.</a></li>
</ul>
  

### Associated credit
<a href="https://github.com/cumuloworks">@cumuloworks</a>' - sequence image manager inspired the conception of this project. 
