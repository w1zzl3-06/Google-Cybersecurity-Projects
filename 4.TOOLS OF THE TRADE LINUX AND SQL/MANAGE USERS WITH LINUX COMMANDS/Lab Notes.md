sudo useradd researcher9

Adds a user called researcher9 to the system.

sudo usermod -g research_team researcher9

Adds researcher9 to the research_team group as their primary group.

sudo useradd researcher9 -g research_team

 A variation of useradd when creating the user to perform both steps at once.

sudo chown researcher9 /home/researcher2/projects/project_r.txt

 Makes researcher9 the owner of /home researcher2/projects project_r.txt.

sudo usermod -a -G sales_team researcher9

Adds researcher9 to the sales_team group as a secondary group.

