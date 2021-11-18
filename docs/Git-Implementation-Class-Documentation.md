---
title: Git-Implementation Class Documentation
---

This document was created by the [PetranWay Autodocumentation Utility](https://bitbucket.org/ChrisCilino/labview-auto-documentation/src/master/).

[TOC]

# Charter

Empty

# Private Data

See the [Class Report Design](https://bitbucket.org/ChrisCilino/labview-auto-documentation/wiki/User%20Documentation/Confluence%20Report%20Printouts/Class) for an explanation of [data name](https://bitbucket.org/ChrisCilino/labview-auto-documentation/wiki/User%20Documentation/Confluence%20Report%20Printouts/Class#markdown-header-private-data-name) and [type](https://bitbucket.org/ChrisCilino/labview-auto-documentation/wiki/User%20Documentation/Confluence%20Report%20Printouts/Class#markdown-header-private-data-type) syntax.

|Name|Description|Data Type|
|-|-|-|
|Git Application||String|
|Top Directory||Path|
|Merge-Delegate||LabVIEW Class of type "Merge-Delegate"|


# Location

C:\PetranWay\Reuse Development\LabVIEW_Git\Implementation\Git Implementation.lvclass

# Members

|Member Name|Scope|Dynamic Dispatch|Must Override|Must Use Parent Implementation|Description|Prototype|
|-|-|-|-|-|-|-|
|CMD Return|community|FALSE|FALSE|FALSE||![CMD Returnc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/CMD%20Returnc.png)|
|Execute Command|community|FALSE|FALSE|FALSE||![Execute Commandc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Execute%20Commandc.png)|
|Add|public|FALSE|FALSE|FALSE|Add specific files from the working tree to the index (stage the files). This operation prepares the index for an upcoming Commit operation.|![Addc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Addc.png)|
|Clone|public|FALSE|FALSE|FALSE|Clone a repository from the Remote URL. The repository will be cloned into the directory specified as the Target Directory, which should be either nonexistent or empty. Do not use the Status Message as a parseable output - it is for user information/display only and may change between versions.|![Clonec.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Clonec.png)|
|Commit|public|FALSE|FALSE|FALSE|Create a new commit containing the current contents of the index.|![Commitc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Commitc.png)|
|Fetch|public|FALSE|FALSE|FALSE|Fetches (updates) a repository from the remote by name or URL. When no name is specified, the default remote will be used (this is often called "origin"). Do not use the Status Message as a parseable output - it is for user information/display only and may change between versions.|![Fetchc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Fetchc.png)|
|Merge|public|FALSE|FALSE|FALSE||![Mergec.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Mergec.png)|
|Push|public|FALSE|FALSE|FALSE|Updates remote refs using local refs, while sending objects necessary to complete the given refs.  Repository can be the name of a remote (e.g. "origin") or a URL. If it is empty, then the value is taken from the configuration for the local repository (via branch.*.remote). If no configuration exists, then "origin" is used).|![Pushc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Pushc.png)|
|Reset|public|FALSE|FALSE|FALSE|Reset the state of the repository based on the Reset Mode and the current state. Hard will modify the local directory to match the Target. Soft will not modify the local directory, but will update HEAD. Mixed will move the HEAD to the Target, and update the index, but will not change the local directory contents.  Alternatively files can be specified to be reset - in this case, the file copies will be copied from Target to the index (what would be commited if a 'Git Commit' immediately followed).|![Resetc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Resetc.png)|
|Message to Message Option|private|FALSE|FALSE|FALSE||![Message to Message Optionc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Message%20to%20Message%20Optionc.png)|
|Parse Push Refspecs|private|FALSE|FALSE|FALSE||![Parse Push Refspecsc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Parse%20Push%20Refspecsc.png)|
|Upstream Error Message|private|FALSE|FALSE|FALSE|Provide a message for the Error case in API operations, when the operation receives an error on the input wire.|![Upstream Error Messagec.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Upstream%20Error%20Messagec.png)|
|Format Paths|protected|TRUE|FALSE|FALSE|Converts an array of paths to a string that can be used to provide a "pathspec" element for Git commands.|![Format Pathsc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Format%20Pathsc.png)|
|Add Options|public|FALSE|FALSE|FALSE|Set of implemented options for the Git Add operation. These settings will not force a configured true option in your gitconfig to be set false - they can only be used to force an option to be used (not not used).  **All**: "--all". Add, modify or remove index entries as needed to match the working tree.  **Force**: "--force". Allow adding ignored files.  **Intent Only**: "--intent-to-add". Don't stage the file - just add an empty object to the index at this path. The path must exist!  **Continue on Error**: "--ignore-errors". Don't abort if an error occurs indexing files. Continue through the full list of files. The return value will still be non-zero if this occurs.|![Add Optionsc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Add%20Optionsc.png)|
|Force Mode|public|FALSE|FALSE|FALSE||![Force Modec.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Force%20Modec.png)|
|Output Type|public|FALSE|FALSE|FALSE||![Output Typec.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Output%20Typec.png)|
|Push Options|public|FALSE|FALSE|FALSE||![Push Optionsc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Push%20Optionsc.png)|
|Reset Mode|public|FALSE|FALSE|FALSE||![Reset Modec.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Reset%20Modec.png)|
|Tag Operation|public|FALSE|FALSE|FALSE||![Tag Operationc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Tag%20Operationc.png)|
|Set Git Application|public|FALSE|FALSE|FALSE||![Set Git Applicationc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Set%20Git%20Applicationc.png)|
|Status|public|FALSE|FALSE|FALSE|Show the working tree status. From git-scm.com/docs/git-status: Displays paths that have differences between the index file and the current HEAD commit, paths that have differences between the working tree and the index file, and paths in the working tree that are not tracked by Git (and are not ignored by gitignore). The first are what you would commit by running git commit; the second and third are what you could commit by running git add before running git commit.|![Statusc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Statusc.png)|
|Tag|public|FALSE|FALSE|FALSE|Create, list, delete or verify the signature of a tag object. By default, use this VI to create annotated tags that can be pushed using Push together with the tags option. A signed tag requires a GnuPG key associated with your committer identity, found via your git-configuration. See https://git-scm.com/docs/git-tag for further details.|![Tagc.png](https:///Developer%20Resources/APIs/Images/Git%20Implementation%20Class%20Documentation/Tagc.png)|

