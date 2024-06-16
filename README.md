# Sticky Notes Resume Theme for Hugo

A swift, minimalist, and responsive Hugo resume theme with sticky-note highlights for essential information.

![example-resume-notes-resume-page](images/demo.webp)

## Features

- Responsive Design: Looks great on all devices.
- Sticky Note Highlights: Essential information stands out like a sticky note.
- Customizable Information: Easily update your phone number, email, LinkedIn profile, and language proficiency information and more.
- Telephone numbere and e-mail addres obsfuction - Your telephone number and e-mail address are not displayed directly on the website. An obsfuction mechanism is used to prevent leakage of your sensitive data.
- Emoji Support: Add personality to your resume with emojis.

## Installation


Add or change hugo config

toml:
```toml
theme = ["github.com/devintrap/sticky-notes-resume"]
#{...}
module:
# {...}
  imports:
  - path: github.com/devintrap/sticky-notes-resume
```

yml:
```yaml
theme: ["github.com/devintrap/sticky-notes-resume"]
#{...}
[module]
# {...}  
  [[module.imports]]
    path = "github.com/devintrap/sticky-notes-resume"
```

update
```bash
hugo mod get -u
```

## Configuration

Check out example [hugo.toml](/hugo.toml.example) or [hugo.yml.example](/hugo.yml)

> Set `markup.goldmark.renderer.unsafe` to `true`  if you want to use `<mark>` inside `_index.md` file.

### List of theme parameters
| Parameter | Description | Default Variable |
|-----------|-------------|------------------|
| `params.resume.name` | Your first name for the resume. | - |
| `params.resume.lastName` | Your last name for the resume. | - |
| `params.resume.location` | Your location as listed on the resume. | - |
| `params.resume.remote` | Indicates if you are open to remote work. | `false` |
| `params.resume.lead` | Describes your professional roles and interests. | - |
| `params.contact.tel` | Your contact telephone number. | - |
| `params.contact.mail` | Your professional email address. | - |
| `params.contact.linkedin` | Your LinkedIn profile URL. | - |
| `params.yearsOfExperience.text` | Describes your experience in software development. | `years of expirence` |
| `params.yearsOfExperience.startDate` | The start date of your software development career. | - |
| `params.languages.text` | Describes the languages you speak. | `Language proficiency` |
| `params.languages.items.lang` | The language spoken. | - |
| `params.languages.items.level` | Your proficiency level in the language. | - |
| `params.skills` | Lists your technical skills relevant to software development. | - |