FROM some-gitlab-registry.example.org/dev/build:base

RUN apt-get update && apt-get upgrade -y && apt-get install -y --no-install-recommends \
		python-nose \
		python-coverage \
		python-mock \
		aida-ui-testing \
		aida-i18n \
	&& rm -rf /var/lib/apt/lists/*

RUN adduser --group --system build
RUN git config --global user.email 'gitlab@example.org' && git config --global user.name "gitlab autobuild"

COPY etc-extras /etc/
COPY build-scripts /usr/local/sbin/
