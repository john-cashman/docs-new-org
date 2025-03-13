# Importing content


You can migrate and unify existing documentation in GitBook using the import tool.

You have the option to import single or multiple pages using our built-in import tool — or [an entire Git repository using Git Sync](import.md#import-using-git-sync) .

## Using the Import Panel


### Supported import formats


GitBook supports imports from websites or files in the following formats:

- Markdown ( or )
- HTML ( )
- Microsoft Word ( )


Markdown ( or )

HTML ( )

Microsoft Word ( )

We also support imports from:

- Confluence
- Notion
- GitHub Wiki
- Quip
- Dropbox Paper
- Google Docs


Confluence

Notion

GitHub Wiki

Quip

Dropbox Paper

Google Docs

GitBook is Markdown-based, so importing content in Markdown format will yield the best results. If your current tools support exporting in Markdown, we recommend using that format for a smoother import process.

### The Import panel


![](image-not-found)

The import panel in GitBook.

When you create a new space, you’ll have the option to import content from the bottom sheet of the first empty page.

Alternatively, you can always import a page or subpage by selecting > in the [table of contents](../resources/gitbook-ui.md#table-of-contents) , or opening the Actions menu for a page and choosing .

![](image-not-found)

After choosing an input source, you can select the file you’d like to import.

GitBook imports content from various sources, but differences in product features and document formats may cause variations in the imported content compared to the original source.

### Limitations


GitBook currently has the following limits for imported content:

- The maximum number of pages that can be uploaded in a single import is .
- The maximum number of files (images etc.) that can be uploaded in a single import is .


The maximum number of pages that can be uploaded in a single import is .

The maximum number of files (images etc.) that can be uploaded in a single import is .

## Import using Git Sync


For importing large volumes of content into GitBook, we recommend using [Git Sync](git-sync/) . Unlike our integrated import tool, Git Sync is better suited for handling larger migrations efficiently.

You’ll find the essential steps to import your content below. For more detailed steps and a video demo, head over to our dedicated guide to [importing content into GitBook using Git Sync](https://app.gitbook.com/s/LBGJKQic7BQYBXmVSjy0/product-guides/import-or-migrate-your-content-to-gitbook-with-git-sync) .

Here’s how to do it:

### Convert your content into Markdown


GitBook is Markdown-based, so importing content in Markdown format will yield the best results. If your current tools support exporting in Markdown, we recommend using that format for a smoother import process.

If your content isn’t already in Markdown files, we recommend using a script (like [Martkitdown](https://github.com/microsoft/markitdown) ) or an online tool to convert your content.

### Organize your content in GitHub or GitLab


When setting up your GitBook site, it’s crucial to organize your content in your GitHub or GitLab repository efficiently. Since Git Sync occurs at the space level, carefully plan how to group your content. Create multiple repositories or folders, ensuring the necessary Markdown files are in the correct locations.

### Set up spaces and Git Sync


To organize your content, create one or more spaces in GitBook as needed. Install the [GitHub Sync](https://www.gitbook.com/integrations/github-sync) or [GitLab Sync](https://www.gitbook.com/integrations/gitlab-sync) integrations in your organization and configure it for those spaces. You’ll need to synchronize your space with the folder or repository you set up in the previous step.

### Run Git Sync in the direction GitHub → GitBook


When following the configuration process, make sure you select the direction of GitHub → GitBook. This will result in the contents of your folder or repository being pulled from GitHub or GitLab into GitBook.