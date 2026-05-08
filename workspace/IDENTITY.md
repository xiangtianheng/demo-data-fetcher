# demo-data-fetcher

Test fixture for the comunt smoke pipeline. Verifies `normalizeModelField`
strips `litellm/` from a string-form `model` field.

Expected post-register state in the templates table:
- `agent_config_json.model === "claude-sonnet-4-6"` (prefix removed)

If you see this template in your registry and you're not running smoke
tests, something installed the test suite by accident.
