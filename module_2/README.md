1.Tēma
Kopsavilkums
1. Jāizveido jauns repozitorijs GitHub - https://github.com/ , kurš satur README.md 
failu
Jānodod: links uz repozitoriju
2. Jāuzstada programmu git no vietnes - https://git-scm.com/ ievērojot jūsu 
operētāj sistēmas prasības 
Ja rodas jautājumi: noskatīties pamācību 
https://www.youtube.com/watch?v=4xqVv2lTo40
Jānodod: bilde no jūsu darba stacijas Windows (Linux vai Mac) ar to ka git ir uzstādīts. 
Palaižot komandu git (Windows : cmd vai Windows PowerShell vai Windows Terminal; 
Linux: bash vai zsh shell; Mac Os: Terminal app)
3. Jāuzstada vienu no koda rediģēšanas programmas no saraksta zemāk:
Visual studio code - https://code.visualstudio.com/
Notepad++ - https://notepad-plus-plus.org/downloads/
Sublime Text - https://www.sublimetext.com/
Atom - https://atom.io/
Jānodod: bilde no jūsu redaktora ar Hello world programmu jebkura programmēšanas 
valoda, kuru pārvaldāt ar attiecīgo stilu.
Materiāli kurus būtu labi apskatīties: 
DevOps tehnoloģiju un riku apkopojums - https://roadmap.sh/devops
Terrafrom ieskats - https://www.hashicorp.com/products/terraform
Ansible ieskats - https://www.redhat.com/en/technologies/management/ansible
Jira par ITIL – https://www.atlassian.com/blog/jira-service-desk/jira-service-desk-itilcertified
Jira par ITSM – https://www.atlassian.com/software/jira/service-management/itsmsoftware
Jira Agile manisfesto - https://www.atlassian.com/agile/manifesto
Jira par Scrum - https://www.atlassian.com/agile/scrum
Jira par Kanban - https://www.atlassian.com/agile/kanban
Jira par Agile un DevOps - https://www.atlassian.com/agile/devops
! Tiem kuri nav pieraduši strādāt ar OS termināliem uzstādīt papildus:
GitHub Desktop - https://desktop.github.com/

Autors Edijs

13.
[ed@testhost dev_ops_kursi]$  git cat-file -p main^{tree}
100644 blob 513cff87ad50e129bf5e52fb687655352ed7381b    README.md
040000 tree fb0e617ff2086e26f815ce0e0cd80c77de1e1a9a    ansible
040000 tree 21a9f6d50a653ad5d4e9d6682cc44e877660b3e5    module_1
040000 tree fb0e617ff2086e26f815ce0e0cd80c77de1e1a9a    terraform
100644 blob 302e1fc83c80daba145df46615e26423793c5a37    test_file

[ed@testhost dev_ops_kursi]$  git cat-file -p 21a9f6d50a653ad5d4e9d6682cc44e877660b3e5
100644 blob e03a8a9b3fca6b8b58826b7710771fecb14e5a6c    README.md

[ed@testhost dev_ops_kursi]$ git hash-object module_1/README.md
e03a8a9b3fca6b8b58826b7710771fecb14e5a6c

[ed@testhost dev_ops_kursi]$ git hash-object module_2/README.md
e03a8a9b3fca6b8b58826b7710771fecb14e5a6c

16. 
git log --since=7.days
git log --pretty="%h - %s" --since="2022-04-18"

17.
git log --pretty="%h - %s" --author='Laura Pacilio'

18.
git log --author='Laura Pacilio' --since="2021-09-01" --until="2021-10-01"

19. 
git log --author='Laura Pacilio' --since="2022-04-25" --until="2022-04-26"
