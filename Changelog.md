# Changes by release

## 0.5.0 unreleased

- Include Debian support only for buster and bookworm.
- Update package `openjdk-11-jre-headless` to `openjdk-17-jre-headless`
in `tasks/apt.yml`.
- Exclude package `libappindicator3-0.1-cil-dev` as dependency in `tasks/apt.yml`.

## 0.4.0 2023-05-26

- Fix missing state in win_chocolatey module.
- Add dependencies information into [meta/main.yml](meta/main.yml).
- Add `win_chocolatey` tag into win_chocolatey task to allow selection of this 
module among ajholanda Galaxy roles.

## [0.3.0] 2023-05-18

- Add variable `package_state` to be used as default and generalized package state value.
- Confine repository state values on *_repository modules.
