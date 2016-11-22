FROM some-gitlab-registry.example.org/gitlab-buildpackage:base

RUN adduser --group --system build
RUN git config --global user.email 'gitlab@example.org' && git config --global user.name "gitlab autobuild"

COPY gbp-envdir /usr/local/gbp-envdir/
COPY etc-extras /etc/
COPY build-scripts /usr/local/sbin/
