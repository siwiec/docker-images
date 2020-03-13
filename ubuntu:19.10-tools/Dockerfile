# docker build -t ubuntu:19.10-tools
# docker run --rm -v $PWD:/workdir --cap-add=SYS_PTRACE --security-opt seccomp=unconfined -d --name ubuntu -i ubuntu:19.10-tools
# docker exec -it ubuntu /bin/bash

FROM ubuntu:19.10

RUN apt-get update
RUN apt-get install -y \
	apktool \
	apt-utils \
	bat \
	build-essential \
	cloc \
	cmake \
	curl \
	gdb \
	ghc \
	git \
	golang-go \
	htop \
	libbz2-dev \
	libffi-dev \
	libreadline-dev \
	libsqlite3-dev \
	libssl-dev \
	locales \
	lsof \
	ltrace \
	make \
	net-tools \
	netcat \
	nmap \
	openvpn \
	python \
	python-openssl \
	python-pip \
	python3 \
	python3-pip \
	radare2 \
	rar \
	rsync \
	screen \
	sed \
	sqlmap \
	strace \
	subversion \
	tcpdump \
	telnet \
	tmux \
	tree \
	unrar \
	unzip \
	vim \
	vpnc \
	wget \
	xxd \
	zip \
	zlib1g-dev

RUN apt-get dist-upgrade -y

WORKDIR /home
RUN git clone https://github.com/pyenv/pyenv.git
ENV PYENV_ROOT "/home/pyenv"
ENV PATH "$PATH:/home/pyenv/bin"
RUN pyenv install 3.8.1
RUN pyenv install 2.7.17
RUN pyenv global 3.8.1
RUN pyenv rehash

RUN pip install \
	jupyter \
	ipython \
	numpy \
	scipy \
	beautifulsoup4 \
	crypto \
	cryptography \
	capstone \
	requests \
	pwntools \
	r2pipe


RUN pip3 install \
	jupyter \
	ipython \
	numpy \
	scipy \
	beautifulsoup4 \
	crypto \
	cryptography \
	capstone \
	requests \
	pwntools \
	r2pipe

# WORKDIR /opt

# RUN git clone https://github.com/0xd4d/dnSpy.git
# RUN git clone https://github.com/1N3/Findsploit.git
# RUN git clone https://github.com/1N3/Goohak.git
# RUN git clone https://github.com/1N3/Sn1per.git
# RUN git clone https://github.com/BinaryAnalysisPlatform/bap.git
# RUN git clone https://github.com/BuffaloWill/oxml_xxe.git
# RUN git clone https://github.com/ChrisTruncer/EyeWitness.git
# RUN git clone https://github.com/D35m0nd142/LFISuite.git
# RUN git clone https://github.com/DataSploit/datasploit.git
# RUN git clone https://github.com/Dionach/CMSmap.git
# RUN git clone https://github.com/EnableSecurity/wafw00f.git
# RUN git clone https://github.com/GoSecure/ysoserial.git
# RUN git clone https://github.com/JacobReynolds/ssrfDetector.git
# RUN git clone https://github.com/JesusFreke/smali.git
# RUN git clone https://github.com/JonathanSalwan/ROPgadget.git
# RUN git clone https://github.com/MobSF/Mobile-Security-Framework-MobSF.git
# RUN git clone https://github.com/OJ/gobuster.git
# RUN git clone https://github.com/OWASP/Amass.git
# RUN git clone https://github.com/RUB-NDS/CORStest.git
# RUN git clone https://github.com/RetireJS/retire.js.git
# RUN git clone https://github.com/UltimateHackers/XSStrike.git
# RUN git clone https://github.com/ZephrFish/GoogD0rker.git
# RUN git clone https://github.com/aboul3la/Sublist3r.git
# RUN git clone https://github.com/ambionics/phpggc.git
# RUN git clone https://github.com/androguard/androguard.git
# RUN git clone https://github.com/angr/angr.git
# RUN git clone https://github.com/anshumanbh/brutesubs.git
# RUN git clone https://github.com/anshumanbh/git-all-secrets.git
# RUN git clone https://github.com/anshumanbh/kubebot.git
# RUN git clone https://github.com/anshumanbh/tko-subs.git
# RUN git clone https://github.com/arthaud/python3-pwntools.git
# RUN git clone https://github.com/auth0/repo-supervisor.git
# RUN git clone https://github.com/awslabs/git-secrets.git
# RUN git clone https://github.com/blechschmidt/massdns.git
# RUN git clone https://github.com/breenmachine/httpscreenshot.git
# RUN git clone https://github.com/bugbountyforum/XSS-Radar.git
# RUN git clone https://github.com/dmayer/idb.git
# RUN git clone https://github.com/drwetter/testssl.sh.git
# RUN git clone https://github.com/dxa4481/truffleHog.git
# RUN git clone https://github.com/enjoiz/XXEinjector.git
# RUN git clone https://github.com/epinna/tplmap.git
# RUN git clone https://github.com/epsylon/xsser.git
# RUN git clone https://github.com/evilsocket/xray.git
# RUN git clone https://github.com/guelfoweb/knock.git
# RUN git clone https://github.com/henshin/filebuster.git
# RUN git clone https://github.com/iBotPeaches/Apktool.git
# RUN git clone https://github.com/infosec-au/altdns.git
# RUN git clone https://github.com/infosec-au/assetnote.git
# RUN git clone https://github.com/insp3ctre/race-the-web.git
# RUN git clone https://github.com/internetwache/GitTools.git
# RUN git clone https://github.com/intrigueio/intrigue-core.git
# RUN git clone https://github.com/java-decompiler/jd-gui.git
# RUN git clone https://github.com/jhaddix/domain.git
# RUN git clone https://github.com/jobertabma/ground-control.git
# RUN git clone https://github.com/kost/dvcs-ripper.git
# RUN git clone https://github.com/lanjelot/patator.git
# RUN git clone https://github.com/lorenzog/dns-parallel-prober.git
# RUN git clone https://github.com/maK-/scantastic-tool.git
# RUN git clone https://github.com/mak-/parameth.git
# RUN git clone https://github.com/mandatoryprogrammer/xsshunter.git
# RUN git clone https://github.com/mandatoryprogrammer/xsshunter_client.git
# RUN git clone https://github.com/maurosoria/dirsearch.git
# RUN git clone https://github.com/mazen160/bfac.git
# RUN git clone https://github.com/mazen160/struts-pwn.git
# RUN git clone https://github.com/mhmdiaa/second-order.git
# RUN git clone https://github.com/michenriksen/gitrob.git
# RUN git clone https://github.com/nahamsec/HostileSubBruteforcer.git
# RUN git clone https://github.com/neex/ffmpeg-avi-m3u-xbin.git
# RUN git clone https://github.com/niklasb/libc-database.git
# RUN git clone https://github.com/penafieljlm/inquisitor.git
# RUN git clone https://github.com/pwndbg/pwndbg.git
# RUN git clone https://github.com/radare/radare2.git
# RUN git clone https://github.com/radareorg/radare2.git
# RUN git clone https://github.com/rajeshmajumdar/BruteXSS.git
# RUN git clone https://github.com/rbsec/dnscan.git
# RUN git clone https://github.com/rezasp/joomscan.git
# RUN git clone https://github.com/shellphish/fuzzer.git
# RUN git clone https://github.com/smicallef/spiderfoot.git
# RUN git clone https://github.com/ticarpi/jwt_tool.git
# RUN git clone https://github.com/urbanadventurer/whatweb.git
# RUN git clone https://github.com/vanhauser-thc/thc-hydra.git
# RUN git clone https://github.com/volatilityfoundation/volatility.git
# RUN git clone https://github.com/vulnersCom/getsploit.git
# RUN git clone https://github.com/xmendez/wfuzz.git
# RUN git clone https://github.com/yaph/domxssscanner.git
# RUN git clone https://github.com/yasinS/sandcastle.git
# RUN git clone https://github.com/ztgrace/changeme.git
