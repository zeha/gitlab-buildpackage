Docker image build scripts
--------------------------

To build and upload to gitlab:

    docker login some-gitlab-registry.example.org
    ./fetch-sources  # downloads repository keys for apt
    ./publish


Assumptions
-----------

  * gitlab-multi-ci-runner with docker runner
  * gitlab docker registry enabled
  * gitlab 8.13+
  * only build for amd64


Notes
-----

Real hostnames have been replaced with \*.example.org.

