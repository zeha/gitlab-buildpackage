FROM buildpack-deps:jessie-curl

COPY keys /etc/apt/trusted.gpg.d/

RUN apt-get update && apt-get upgrade -y && apt-get install -y --no-install-recommends \
		equivs \
		openssh-client \
		pep8 \
		build-essential \
		devscripts \
		dpkg-dev \
		fakeroot \
		git-buildpackage \
		lintian \
		pristine-tar \
		runit \
		aptitude \
		ca-certificates \
		apt-utils \
	&& rm -rf /var/lib/apt/lists/*
