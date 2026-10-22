# ai-tools

Reusable skills for GitHub Copilot, packaged as an installable plugin. The plugin currently includes `report-bc-translation-defect`.

## Install

### VS Code

In Copilot Chat, run:

```text
/plugin install https://github.com/nicolassaleron/ai-tools
```

Alternatively, open the Command Palette and select **Chat: Install Plugin From Source**, then enter `https://github.com/nicolassaleron/ai-tools`.

### GitHub Copilot CLI

Register this repository as a marketplace, then install its plugin:

```sh
copilot plugin marketplace add nicolassaleron/ai-tools
copilot plugin install ai-tools@ai-tools
```

The CLI installs plugins by marketplace identity, so it does not use `copilot plugin install OWNER/REPO` directly. To confirm the installation, run `copilot plugin list`.

After installation, use `/report-bc-translation-defect` in Copilot Chat, or let Copilot load the skill when the task matches its description. Review the skill's `SKILL.md` before use.

See the [VS Code Agent Plugins documentation](https://code.visualstudio.com/docs/agent-customization/agent-plugins) and [Copilot CLI plugin documentation](https://docs.github.com/en/copilot/how-tos/copilot-cli/customize-copilot/plugins-finding-installing) for more details.