# vcd-v2t
```
 curl -LsSf https://astral.sh/uv/install.sh | sh
  export PATH=$PATH:$HOME/.local/bin
  uv venv
  source .venv/bin/activate
  uv pip install -r requirements_build.txt
  uv pip install -r src/requirements.txt
  uv run python -m PyInstaller src/vcdNSXMigrator.spec
  export LINUX_PACKAGE="VMware-NSX-Migration-for-VMware-Cloud-Director-$RELEASE_VERSION-Ubuntu.tar.gz"
  tar -czvf $LINUX_PACKAGE -C dist/ .
```
