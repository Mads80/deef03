+++
date = '2026-07-05T22:58:41+02:00'
draft = false
title = 'Enter the Massgrave'
tags = ['massgrave', 'windows', 'win11', 'fedora', 'linux', 'piracy']
showAuthor = false
+++

>Let's be real. *Nobody* likes Windows, and even fewer likes paying for it. Enter the Massgrave.
>![Pirate Flag](img/pirate-flag.png)

## Howto

Copy and paste the code below into your PowerShell terminal:
```powershell
irm https://get.activated.win | iex
```

Follow the prompts and the script will take care of the rest.

> [!NOTE]
> The `irm` command in PowerShell downloads a script from a specified URL, and the `iex` command executes it.
>
> Always double-check the URL before executing the command and verify the source is trustworthy when manually downloading files.

> [!TIP]
> You can install Windows without setting up an account. Hit `Shift + F10` during the installation process to bring up the command prompt and type `start ms-cxh:localonly`. This will immediately bypass the Microsoft Account requirement and open the local user creation screen.

---

## With that out of the way, what is Massgrave?

Well, daunting name aside, it’s an open-source Windows activation script that uses a combination of techniques to bypass Microsoft’s activation requirements.

For more information, see the [GitHub repository](https://github.com/massgravel/Microsoft-Activation-Scripts). And remember, GitHub is owned by Microsoft. And still, the script remains on GitHub.

{{< github repo="massgravel/Microsoft-Activation-Scripts" showThumbnail=false >}}

Got any questions? Make sure to read the [FAQ](https://massgrave.dev/faq).

> [!WARNING]
> Keep in mind that this goes against Microsoft's Terms of Service. Legal rules differ depending on where you live, so make sure you understand the risks in your area.

---

## Is it safe?

This question have been asked multiple times before, here's a [summary](https://massgrave.dev/faq#is-mas-safe).

> [!QUOTE]
> MAS is fully open-source, with over 150K stars on GitHub and millions of users worldwide. You can open the batch files in Notepad to review the code yourself, or ask others who have already reviewed the code.

Link to one of many Reddit threads on the topic: [Is Masgrave really safe?](https://www.reddit.com/r/WindowsLTSC/comments/1omt5s2/is_masgrave_really_safe)

> [!QUOTE]
> Massgrave is hosted on a website owned by Microsoft themselves (GitHub) for more than 10 years and their technical support uses it themselves – if you have trouble activating your legitimate Windows license for example, their team will often use Massgrave to activate Windows. If that isn’t safe I don’t know what is. 

---

## Alternative Solutions

If you're not totally sold on pirating Windows, you might want to consider alternative solutions, like the [Fedora Workstation](https://getfedora.org/workstation/). with the GNOME desktop environment. The GNOME desktop environment is very clean and modern, and it runs incredibly well.

Other alternatives include the [Ubuntu desktop environment](https://ubuntu.com/), or [Linux Mint](https://linuxmint.com/). Both are very popular and have a large community of users.
