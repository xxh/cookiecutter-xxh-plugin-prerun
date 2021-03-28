Cookiecutter template to create xxh-plugin-prerun.

# Example

```python
pip install cookiecutter

cookiecutter gh:xxh/cookiecutter-xxh-plugin-prerun
# github_username [username]: xxh
# project_name [my-tool]: zoxide
# project_repo_name [xxh-plugin-prerun-zoxide]: <ENTER>
# project_short_description [The my-tool for xxh.]: Using zoxide in xxh.

tree xxh-plugin-prerun-zoxide
# xxh-plugin-prerun-zoxide/
# ├── build.sh
# ├── LICENSE
# ├── prerun.sh
# ├── README.md
# └── requirements.txt
```

# Integration with xxh-shells

To integrate the plugin with xxh-shell create `pluginrc` file. For example create `pluginrc.zsh` with the content to init the zoxide:
```shell
eval "$(zoxide init zsh)"
```