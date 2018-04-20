bootstrap: docker
from: ubuntu:16.04

%runscript

  git "$@"


%post
  apt-get update
  apt-get install -y git wget

  cd /
  wget https://github.com/git-lfs/git-lfs/releases/download/v2.4.0/git-lfs-linux-amd64-2.4.0.tar.gz
  tar -xzf *.tar.gz
  cd git-lfs*
  ./install.sh
  git lfs install
