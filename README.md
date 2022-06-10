# Task-1
 $ wget https://raw.githubusercontent.com/HackBio-Internship/wale-home-tasks/main/DNA.fa 
 $ grep '>' DNA.fa | wc -l
$ grep -v ">" DNA.fa | grep -E -o "G|C|T|A" | wc -l 
$ wget https://repo.anaconda.com/miniconda/Miniconda3-py38_4.12.0-Linux-x86_64.sh
$ chmod +x Miniconda3-py38_4.12.0-Linux-x86_64.sh
$ ./Miniconda3-py38_4.12.0-Linux-x86_64.sh

$ wget https://github.com/josoga2/yt-dataset/blob/516b13bca08ab2c4bcaf58d6ffc48e16c2996554/dataset/raw_reads/Chara_R1.fastq.gz

$ wget https://github.com/josoga2/yt-dataset/blob/516b13bca08ab2c4bcaf58d6ffc48e16c2996554/dataset/raw_reads/Chara_R2.fastq.gz
$ mkdir output
wget http://cab.spbu.ru/files/release3.12.0/SPAdes-3.12.0-Linux.tar.gz tar -xzf SPAdes-3.12.0-Linux.tar.gz cd SPAdes-3.12.0-Linux/bin/
spades.py -1 Chara_R1.fastq.gz -2 Chara_R2.fastq.gz –careful –cov –cutoff auto -o output 
