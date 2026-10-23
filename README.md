### Hi there 👋

## I'm Abhishek, an Android engineer

- 📱 I build Android apps with Kotlin, Jetpack Compose and Clean Architecture
- 🚀 I automate mobile release chores — versioning, release notes, store rollouts — with Gradle and GitHub Actions
- 🌱 I'm currently learning agent programming
- ⚡ Fun fact: I love watching anime and reading manga

### Mobile CI/CD toolkit 🧰

GitHub Actions I maintain for Android and iOS release pipelines. Each one has tests, CI and ready-to-copy example workflows.

#### Versioning and planning

| Action | What it does |
|:-------|:-------------|
| [mobile-version-bump](https://github.com/abhishek-3289/mobile-version-bump) | Bumps Android and iOS versions and build numbers together from the latest git tag (`version.properties`, `build.gradle`, `.xcconfig`, `project.pbxproj`, `Info.plist`). |
| [android-version-increment](https://github.com/abhishek-3289/android-version-increment) | Bumps an Android app's semantic version from the latest git tag via the Gradle semver plugin. |
| [milestone-version-increment](https://github.com/abhishek-3289/milestone-version-increment) | Creates the next semver milestone with an optional prefix, due date and description. |

#### Release and store

| Action | What it does |
|:-------|:-------------|
| [store-release-notes](https://github.com/abhishek-3289/store-release-notes) | Builds Google Play and App Store "What's new" text from merged pull requests, within each store's length limit. |
| [play-rollout-manager](https://github.com/abhishek-3289/play-rollout-manager) | Advances Google Play staged rollouts on a schedule, with weekday-only steps, deployment history, Slack alerts and safety checks. |
| [appstore-phased-release](https://github.com/abhishek-3289/appstore-phased-release) | Pauses, resumes or completes App Store phased releases, with an optional crash-free-rate guard. |

#### Quality

| Action | What it does |
|:-------|:-------------|
| [app-size-report](https://github.com/abhishek-3289/app-size-report) | Compares APK, AAB and IPA sizes against the base branch and keeps a size report comment on the pull request. |

<details>
  <summary>How they fit together</summary>
  <br/>

```text
cut release  ─▶ mobile-version-bump ─▶ milestone-version-increment
PR checks    ─▶ app-size-report
QA sign-off  ─▶ store-release-notes ─▶ upload to Play / App Store
after launch ─▶ play-rollout-manager · appstore-phased-release
```

</details>

### Languages and Tools 🛠️

[![Languages and tools](https://skillicons.dev/icons?i=kotlin,java,androidstudio,gradle,githubactions,nodejs,bash,git&perline=8)](https://skillicons.dev)

<details>
  <summary>⚡ GitHub Stats</summary>
  <br/>
  <img alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=abhishek-3289&hide=contribs,prs&count_private=true&show_icons=true&hide_border=true&custom_title=Stats" />
</details>
