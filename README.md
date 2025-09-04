# llama-stack-trustryai-openshift

## Local run
```shell
python3.12 -m venv .venv
source .venv/bin/activate

pip install -r requirements.txt

export TRUSTYAI_FMS_ORCHESTRATOR_URL=<>
export GRANITE_URL=<>
export QWEN_URL=<>
export REMOTE_OCP_MCP_URL=<>
export REMOTE_SLACK_MCP_URL=<>
export GRANITE_MODEL=granite
export QWEN_MODEL=qwen
export STORE_DIR=./.app-data
export TELEMETRY_SINKS=console

llama stack run llama-stack/local/runtime_configurations/orchestrator_api.yaml --image-type=venv
```
