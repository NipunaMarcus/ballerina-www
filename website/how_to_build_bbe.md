# How to build BBE

This will guide you through the process of using the `build-bbe.sh` tool to generate BBEs as html.

### How to run

from the `website` directory run the following command.

```bash
sudo ./tools/build-bbe.sh <site_version> <output_dir> <ballerina_repo_tag> <generateWithJekyll>
```

**site_version**

This is the version of the site that the tool should generate the BBEs for.
Ex: v1-2 or v1-1

**output_dir**

This is the output directory where the tool will save the generated BBEs html files.

**ballerina_repo_tag**

This is the Ballerina tag that the examples should be extracted from and then use to generate
the BBEs.

Ex: v1.2.0 or v1.1.0.

**generateWithJekyll**

This is the flag to indicate the tool to generate BBEs with or without jekyll front matter.

If pass in `true` it will generate BBEs with jekyll front matter.
If pass in `false` it will generate BBEs without jekyll front matter but as a normal html file.


##### Example Usage

* When building examples for website.

```bash
sudo ./tools/build-bbe.sh v1-2 bbes v1.2.0 true
```

This will generate BBE with jekyll front matter.

* When building examples for normal use.

```bash
sudo ./tools/build-bbe.sh v1-2 bbes v1.2.0 false
```

This will generate BBE without jekyll front matter but as plain html.

