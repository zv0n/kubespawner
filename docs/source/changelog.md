# Changes in KubeSpawner

<!-- PR summaries generated using github-activity CLI, see RELEASE.md for details -->

## [Unreleased]

## 4.1

### [4.1.0] - 2022-05-19

#### New features added

- Support dropdown list choices for `profile_list` profiles via `profile_options` [#607](https://github.com/jupyterhub/kubespawner/pull/607) ([@yuvipanda](https://github.com/yuvipanda))

#### Maintenance and upkeep improvements

- [pre-commit.ci] pre-commit autoupdate [#608](https://github.com/jupyterhub/kubespawner/pull/608) ([@pre-commit-ci](https://github.com/pre-commit-ci))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2022-04-23&to=2022-05-19&type=c))

[@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2022-04-23..2022-05-19&type=Issues) | [@keniseli](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Akeniseli+updated%3A2022-04-23..2022-05-19&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Apre-commit-ci+updated%3A2022-04-23..2022-05-19&type=Issues) | [@rabernat](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Arabernat+updated%3A2022-04-23..2022-05-19&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2022-04-23..2022-05-19&type=Issues)

## 4.0

### [4.0.0] - 2022-04-23

#### Breaking changes

- Support for use against k8s 1.17-1.19 is no longer maintained, please upgrade to k8s 1.20+ to ensure function.
- If you have configured `c.JupyterHub.proxy_class` to use `KubeIngressProxy`, please read the notes in [#598](https://github.com/jupyterhub/kubespawner/pull/598) along with the [disclaimer for use of this JupyterHub proxy class](https://github.com/jupyterhub/kubespawner/blob/ea9a13b73e793574a1a5045be75930122c5b03c9/kubespawner/proxy.py#L44-L75).

#### New features added

- Add `services_enabled` to create a k8s Service for each user pod (enables use with Istio mTLS) [#522](https://github.com/jupyterhub/kubespawner/pull/522) ([@JJ11teen](https://github.com/JJ11teen))

#### Bugs fixed

- [KubeIngressProxy] breaking: Migrate to networking.k8s.io/v1 api for Ingress resources [#598](https://github.com/jupyterhub/kubespawner/pull/598) ([@consideRatio](https://github.com/consideRatio))

#### Maintenance and upkeep improvements

- pre-commit: replace reorder-python-imports with isort [#606](https://github.com/jupyterhub/kubespawner/pull/606) ([@consideRatio](https://github.com/consideRatio))

#### Continuous integration

- ci: stop testinging 1.17-1.19, assume k8s 1.20+ going onwards [#599](https://github.com/jupyterhub/kubespawner/pull/599) ([@consideRatio](https://github.com/consideRatio))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2022-03-15&to=2022-04-23&type=c))

[@agt](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aagt+updated%3A2022-03-15..2022-04-23&type=Issues) | [@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2022-03-15..2022-04-23&type=Issues) | [@JJ11teen](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AJJ11teen+updated%3A2022-03-15..2022-04-23&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2022-03-15..2022-04-23&type=Issues) | [@zflamig](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Azflamig+updated%3A2022-03-15..2022-04-23&type=Issues)

## 3.0

### [3.0.2] - 2022-03-15

#### Bugs fixed

- [KubeIngressProxy] Fix critical regression from typo [#593](https://github.com/jupyterhub/kubespawner/pull/593) ([@ondave](https://github.com/ondave), [@yuvipanda](https://github.com/yuvipanda), [@consideRatio](https://github.com/consideRatio))

#### Maintenance and upkeep improvements

- refactor: add pre-commit hook pyupgrade, and run it [#586](https://github.com/jupyterhub/kubespawner/pull/586) ([@consideRatio](https://github.com/consideRatio))

#### Documentation improvements

- DOCS: Update theme to use book theme [#591](https://github.com/jupyterhub/kubespawner/pull/591) ([@choldgraf](https://github.com/choldgraf), [@consideRatio](https://github.com/consideRatio))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2022-03-14&to=2022-03-15&type=c))

[@choldgraf](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Acholdgraf+updated%3A2022-03-14..2022-03-15&type=Issues) | [@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2022-03-14..2022-03-15&type=Issues) | [@ondave](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aondave+updated%3A2022-03-14..2022-03-15&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2022-03-14..2022-03-15&type=Issues)

### [3.0.1] - 2022-03-14

#### Bugs fixed

- Fix typo in reflector.\_stopping [#587](https://github.com/jupyterhub/kubespawner/pull/587) ([@minrk](https://github.com/minrk), [@consideRatio](https://github.com/consideRatio))

### [3.0.0] - 2022-03-14

This release replaces a synchronous Kubernetes client library with an async
alternative, allowing the use of native Python async features.

#### Breaking changes

- Support for Python 3.6 dropped
- The configuration `k8s_api_threadpool_workers` is removed as we don't create
  threads any more, but now instead relies on scheduling everything to run in an
  event loop.
- A dependency on the library
  [`kubernetes`](https://github.com/kubernetes-client/python#readme) is replaced
  with a dependency on the library
  [`kubernetes_asyncio`](https://github.com/tomplus/kubernetes_asyncio#readme).
- Methods considered internal to Kubespawner are now prefixed with `_`.

#### Maintenance and upkeep improvements

- Please flake8 by removing unused imports [#584](https://github.com/jupyterhub/kubespawner/pull/584) ([@consideRatio](https://github.com/consideRatio))
- close shared clients when loop closes [#579](https://github.com/jupyterhub/kubespawner/pull/579) ([@minrk](https://github.com/minrk), [@consideRatio](https://github.com/consideRatio))
- Simplify async init [#576](https://github.com/jupyterhub/kubespawner/pull/576) ([@minrk](https://github.com/minrk), [@consideRatio](https://github.com/consideRatio))
- Replace recommonmark with myst_parser and fix changelog rendering [#575](https://github.com/jupyterhub/kubespawner/pull/575) ([@rccern](https://github.com/rccern), [@consideRatio](https://github.com/consideRatio), [@welcome](https://github.com/welcome), [@choldgraf](https://github.com/choldgraf), [@manics](https://github.com/manics))
- \[KubeIngressProxy\] Add underscore prefix to private functions: `safe_name_for_routespec` and `delete_if_exists` [#572](https://github.com/jupyterhub/kubespawner/pull/572) ([@consideRatio](https://github.com/consideRatio), [@manics](https://github.com/manics), [@minrk](https://github.com/minrk))
- Misc maintenance details [#571](https://github.com/jupyterhub/kubespawner/pull/571) ([@consideRatio](https://github.com/consideRatio), [@minrk](https://github.com/minrk))
- Rely on the event loop: use `kubernetes_asyncio` instead of `kubernetes` and dedicated threads [#563](https://github.com/jupyterhub/kubespawner/pull/563) ([@athornton](https://github.com/athornton), [@yuvipanda](https://github.com/yuvipanda), [@consideRatio](https://github.com/consideRatio), [@minrk](https://github.com/minrk), [@manics](https://github.com/manics))

#### Documentation improvements

- \[KubeIngressProxy\] Add a long docstring to KubeIngressProxy class [#568](https://github.com/jupyterhub/kubespawner/pull/568) ([@consideRatio](https://github.com/consideRatio), [@yuvipanda](https://github.com/yuvipanda), [@GeorgianaElena](https://github.com/GeorgianaElena))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2022-02-15&to=2022-03-11&type=c))

[@athornton](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aathornton+updated%3A2022-02-15..2022-03-11&type=Issues) | [@choldgraf](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Acholdgraf+updated%3A2022-02-15..2022-03-11&type=Issues) | [@clkao](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aclkao+updated%3A2022-02-15..2022-03-11&type=Issues) | [@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2022-02-15..2022-03-11&type=Issues) | [@GeorgianaElena](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AGeorgianaElena+updated%3A2022-02-15..2022-03-11&type=Issues) | [@manics](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Amanics+updated%3A2022-02-15..2022-03-11&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aminrk+updated%3A2022-02-15..2022-03-11&type=Issues) | [@rccern](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Arccern+updated%3A2022-02-15..2022-03-11&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Awelcome+updated%3A2022-02-15..2022-03-11&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2022-02-15..2022-03-11&type=Issues)

## 2.0

### [2.0.1] - 2022-02-15

#### Maintenance and upkeep improvements

- Support recent version of kubernetes client library (21.7.0) that introduced a breaking change [#558](https://github.com/jupyterhub/kubespawner/pull/558) ([@athornton](https://github.com/athornton))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2021-11-28&to=2022-02-03&type=c))

[@athornton](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aathornton+updated%3A2021-11-28..2022-02-03&type=Issues) | [@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2021-11-28..2022-02-03&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aminrk+updated%3A2021-11-28..2022-02-03&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2021-11-28..2022-02-03&type=Issues)

### [2.0.0] - 2021-11-28

#### Breaking changes

A breaking change was introduced in [#545](https://github.com/jupyterhub/kubespawner/pull/545), making the default value of `allow_privilege_escalation` be `False`. This means a user can't use `sudo` unless `allow_privilege_escalation` is explicitly set to `True`. The JupyterHub user Pod that KubeSpawner creates will have a container with a `securityContext` that has `allowPrivilegeEscalation` set to `false` by default.

For reference, the following can be read about `allowPrivilegeEscalation` in [Kubernetes official documentation](https://kubernetes.io/docs/tasks/configure-pod-container/security-context/):

> AllowPrivilegeEscalation: Controls whether a process can gain more privileges than its parent process. This bool directly controls whether the `no_new_privs` flag gets set on the container process. AllowPrivilegeEscalation is true always when the container is: 1) run as `Privileged` OR 2) has `CAP_SYS_ADMIN`.

To revert to the previous behavior of using the cluster's default, set `allow_privilege_escalation` explicitly to `None`.

#### Bugs fixed

- Default allow_privilege_escalation to False [#545](https://github.com/jupyterhub/kubespawner/pull/545) ([@yuvipanda](https://github.com/yuvipanda))
- Ensure that the \_start_future attribute exists. [#541](https://github.com/jupyterhub/kubespawner/pull/541) ([@athornton](https://github.com/athornton))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2021-11-03&to=2021-11-19&type=c))

[@athornton](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aathornton+updated%3A2021-11-03..2021-11-19&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aminrk+updated%3A2021-11-03..2021-11-19&type=Issues) | [@mriedem](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Amriedem+updated%3A2021-11-03..2021-11-19&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Awelcome+updated%3A2021-11-03..2021-11-19&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2021-11-03..2021-11-19&type=Issues)

## 1.1

### [1.1.2] - 2021-11-03

#### Bugs fixed

- Fix race condition between spawn() calling \_start() and progress() [#511](https://github.com/jupyterhub/kubespawner/pull/511) ([@consideRatio](https://github.com/consideRatio))

#### Maintenance and upkeep improvements

- Rename master to main [#535](https://github.com/jupyterhub/kubespawner/pull/535) ([@consideRatio](https://github.com/consideRatio))
- Remove .pylintrc config [#534](https://github.com/jupyterhub/kubespawner/pull/534) ([@consideRatio](https://github.com/consideRatio))
- Warn about cli args being ignored when KubeSpawner.cmd is not set [#533](https://github.com/jupyterhub/kubespawner/pull/533) ([@minrk](https://github.com/minrk))

#### Other merged PRs

- ci: misc fixes, don't run tests on markdown changes, etc [#539](https://github.com/jupyterhub/kubespawner/pull/539) ([@consideRatio](https://github.com/consideRatio))
- docs: require sphinx >=2 [#538](https://github.com/jupyterhub/kubespawner/pull/538) ([@consideRatio](https://github.com/consideRatio))
- [pre-commit.ci] pre-commit autoupdate [#537](https://github.com/jupyterhub/kubespawner/pull/537) ([@pre-commit-ci](https://github.com/pre-commit-ci))
- Update our docs config [#536](https://github.com/jupyterhub/kubespawner/pull/536) ([@consideRatio](https://github.com/consideRatio))
- [pre-commit.ci] pre-commit autoupdate [#530](https://github.com/jupyterhub/kubespawner/pull/530) ([@pre-commit-ci](https://github.com/pre-commit-ci))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2021-10-04&to=2021-11-03&type=c))

[@athornton](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aathornton+updated%3A2021-10-04..2021-11-03&type=Issues) | [@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2021-10-04..2021-11-03&type=Issues) | [@manics](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Amanics+updated%3A2021-10-04..2021-11-03&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aminrk+updated%3A2021-10-04..2021-11-03&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Apre-commit-ci+updated%3A2021-10-04..2021-11-03&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2021-10-04..2021-11-03&type=Issues)

### [1.1.1] - 2021-10-04

#### Bugs fixed

- Terminate process correctly from reflector thread [#525](https://github.com/jupyterhub/kubespawner/pull/525) ([@yuvipanda](https://github.com/yuvipanda))

#### Continuous integration

- [pre-commit.ci] pre-commit autoupdate [#526](https://github.com/jupyterhub/kubespawner/pull/526) ([@pre-commit-ci](https://github.com/pre-commit-ci))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2021-07-21&to=2021-10-04&type=c))

[@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2021-07-21..2021-10-04&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2021-07-21..2021-10-04&type=Issues)

### [1.1.0] - 2021-07-21

#### Enhancements made

- Expand username etc. in configured service_account [#518](https://github.com/jupyterhub/kubespawner/pull/518) ([@consideRatio](https://github.com/consideRatio))
- Sort env to reliably expand nested env references [#510](https://github.com/jupyterhub/kubespawner/pull/510) ([@consideRatio](https://github.com/consideRatio))

#### Bugs fixed

- Ensure to omit empty lists in security contexts [#517](https://github.com/jupyterhub/kubespawner/pull/517) ([@consideRatio](https://github.com/consideRatio))

#### Maintenance and upkeep improvements

- Generalize omit_namespace functionality [#514](https://github.com/jupyterhub/kubespawner/pull/514) ([@droctothorpe](https://github.com/droctothorpe))
- Remove unneeded dep [#508](https://github.com/jupyterhub/kubespawner/pull/508) ([@dhirschfeld](https://github.com/dhirschfeld))

#### Documentation improvements

- Fix the errors followed by the contributing steps [#509](https://github.com/jupyterhub/kubespawner/pull/509) ([@mggger](https://github.com/mggger))

#### Other merged PRs

- [KubeIngressProxy] Set configuration before instantiating reflectors [#515](https://github.com/jupyterhub/kubespawner/pull/515) ([@droctothorpe](https://github.com/droctothorpe))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2021-05-14&to=2021-07-21&type=c))

[@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2021-05-14..2021-07-18&type=Issues) | [@dhirschfeld](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Adhirschfeld+updated%3A2021-05-14..2021-07-18&type=Issues) | [@droctothorpe](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Adroctothorpe+updated%3A2021-05-14..2021-07-18&type=Issues) | [@mggger](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Amggger+updated%3A2021-05-14..2021-07-18&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2021-05-14..2021-07-18&type=Issues)

## 1.0

### [1.0.0] - 2021-05-14

This release is the continuation of version 0.16.1 and could have been 0.17.0 in
practice. We opted to release 1.0.0 as it enables us to communicate changes
according to [SemVer](https://semver.org/). Using SemVer versioning, a change in
each of the three version numbers (major.minor.patch) represents a different
kind of change.

#### Breaking changes

- When using KubeSpawner 1.0.0 or later together with JupyterHub 1.4.1 or later,
  deleting a JupyterHub user or deleting (not just stopping) a named server will
  lead to removing the associated PVC resource. To opt out of this behavior set
  the `delete_pvc` configuration to `False`.

#### New features added

- Allow configuration of kubernetes client's options: ssl_ca_cert, host [#494](https://github.com/jupyterhub/kubespawner/pull/494) ([@kafonek](https://github.com/kafonek))
- add method to delete namespaced PVC in spawner base class [#475](https://github.com/jupyterhub/kubespawner/pull/475) ([@nsshah1288](https://github.com/nsshah1288))

#### Enhancements made

- Add options_from_form as configurable [#477](https://github.com/jupyterhub/kubespawner/pull/477) ([@cbanek](https://github.com/cbanek))

#### Maintenance and upkeep improvements

- Add MANIFEST.in (LICENCE, README.md) [#495](https://github.com/jupyterhub/kubespawner/pull/495) ([@dhirschfeld](https://github.com/dhirschfeld))

#### Documentation improvements

- Rewrite help for Kubespawner.cmd [#502](https://github.com/jupyterhub/kubespawner/pull/502) ([@manics](https://github.com/manics))

#### Continuous integration

- ci: test against recent k8s versions and misc workflow updates [#506](https://github.com/jupyterhub/kubespawner/pull/506) ([@consideRatio](https://github.com/consideRatio))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2021-03-01&to=2021-05-13&type=c))

[@cbanek](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Acbanek+updated%3A2021-03-01..2021-05-13&type=Issues) | [@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2021-03-01..2021-05-13&type=Issues) | [@dhirschfeld](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Adhirschfeld+updated%3A2021-03-01..2021-05-13&type=Issues) | [@jabbera](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ajabbera+updated%3A2021-03-01..2021-05-13&type=Issues) | [@kafonek](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Akafonek+updated%3A2021-03-01..2021-05-13&type=Issues) | [@manics](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Amanics+updated%3A2021-03-01..2021-05-13&type=Issues) | [@meeseeksmachine](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ameeseeksmachine+updated%3A2021-03-01..2021-05-13&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aminrk+updated%3A2021-03-01..2021-05-13&type=Issues) | [@nsshah1288](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ansshah1288+updated%3A2021-03-01..2021-05-13&type=Issues) | [@octavd](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aoctavd+updated%3A2021-03-01..2021-05-13&type=Issues)

## 0.16

### [0.16.1] - 2021-03-01

#### Bugs fixed

- fix url-change detection in poll [#489](https://github.com/jupyterhub/kubespawner/pull/489) ([@minrk](https://github.com/minrk))

#### Contributors to this release

[@minrk](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aminrk+updated%3A2021-02-26..2021-03-01&type=Issues)

### [0.16.0] - 2021-02-26

#### Enhancements made

- Add pod_security_context and container_security_context config [#480](https://github.com/jupyterhub/kubespawner/pull/480) ([@cyrilcros](https://github.com/cyrilcros))
- Allow mounting of service account token to be configurable (automount_service_account_token) [#476](https://github.com/jupyterhub/kubespawner/pull/476) ([@dtaniwaki](https://github.com/dtaniwaki))
- Add user namespace support [#458](https://github.com/jupyterhub/kubespawner/pull/458) ([@athornton](https://github.com/athornton))
- Support internal_ssl [#409](https://github.com/jupyterhub/kubespawner/pull/409) ([@minrk](https://github.com/minrk))

#### Bugs fixed

- Fix failure to create a PVC being logged as failure to create a Pod [#481](https://github.com/jupyterhub/kubespawner/pull/481) ([@mriedem](https://github.com/mriedem))
- handle pod url changes in poll [#408](https://github.com/jupyterhub/kubespawner/pull/408) ([@minrk](https://github.com/minrk))

#### Maintenance and upkeep improvements

- Refactor: remove a third way to name the same thing in make_pod's parameters [#483](https://github.com/jupyterhub/kubespawner/pull/483) ([@consideRatio](https://github.com/consideRatio))
- pre-commit: use prettier as autoformatter (markdown, yaml) [#482](https://github.com/jupyterhub/kubespawner/pull/482) ([@consideRatio](https://github.com/consideRatio))
- fix some spurious additions in tests [#474](https://github.com/jupyterhub/kubespawner/pull/474) ([@minrk](https://github.com/minrk))
- adopt black (via pre-commit) for code formatting [#473](https://github.com/jupyterhub/kubespawner/pull/473) ([@minrk](https://github.com/minrk))
- remove duplicated secret_mount_path definition [#472](https://github.com/jupyterhub/kubespawner/pull/472) ([@minrk](https://github.com/minrk))

#### Other merged PRs

- [KubeIngressProxy] Fixes following changes to k8s resource reflectors [#484](https://github.com/jupyterhub/kubespawner/pull/484) ([@remche](https://github.com/remche))
- [KubeIngressProxy] allow singleuser pods to use IPv6 addresses [#403](https://github.com/jupyterhub/kubespawner/pull/403) ([@stv0g](https://github.com/stv0g))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2020-12-15&to=2021-02-26&type=c))

[@athornton](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aathornton+updated%3A2020-12-15..2021-02-26&type=Issues) | [@betatim](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Abetatim+updated%3A2020-12-15..2021-02-26&type=Issues) | [@clkao](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aclkao+updated%3A2020-12-15..2021-02-26&type=Issues) | [@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2020-12-15..2021-02-26&type=Issues) | [@cyrilcros](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Acyrilcros+updated%3A2020-12-15..2021-02-26&type=Issues) | [@dhirschfeld](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Adhirschfeld+updated%3A2020-12-15..2021-02-26&type=Issues) | [@dtaniwaki](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Adtaniwaki+updated%3A2020-12-15..2021-02-26&type=Issues) | [@lresende](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Alresende+updated%3A2020-12-15..2021-02-26&type=Issues) | [@manics](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Amanics+updated%3A2020-12-15..2021-02-26&type=Issues) | [@meeseeksmachine](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ameeseeksmachine+updated%3A2020-12-15..2021-02-26&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aminrk+updated%3A2020-12-15..2021-02-26&type=Issues) | [@mriedem](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Amriedem+updated%3A2020-12-15..2021-02-26&type=Issues) | [@remche](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aremche+updated%3A2020-12-15..2021-02-26&type=Issues) | [@shanestarcher-okta](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ashanestarcher-okta+updated%3A2020-12-15..2021-02-26&type=Issues) | [@stv0g](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Astv0g+updated%3A2020-12-15..2021-02-26&type=Issues) | [@tirumerla](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Atirumerla+updated%3A2020-12-15..2021-02-26&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2020-12-15..2021-02-26&type=Issues)

## 0.15

### [0.15.0] - 2020-10-15

#### Enhancements made

- Expand storage selector [#463](https://github.com/jupyterhub/kubespawner/pull/463) ([@dtaniwaki](https://github.com/dtaniwaki))
- Add pod_connect_ip config regarding how kubespawner reach the pod [#460](https://github.com/jupyterhub/kubespawner/pull/460) ([@dtaniwaki](https://github.com/dtaniwaki))
- [Feature] Add AllowPrivilegeEscalation to container's securityContext [#450](https://github.com/jupyterhub/kubespawner/pull/450) ([@captnbp](https://github.com/captnbp))

#### Bugs fixed

- Wrap concurrent.futures Future in polling function [#467](https://github.com/jupyterhub/kubespawner/pull/467) ([@ondave](https://github.com/ondave))
- Let uid/gid/fs_gid default to None instead of 0 [#453](https://github.com/jupyterhub/kubespawner/pull/453) ([@consideRatio](https://github.com/consideRatio))

#### Maintenance and upkeep improvements

- action-k3s-helm was moved to jupyterhub [#465](https://github.com/jupyterhub/kubespawner/pull/465) ([@manics](https://github.com/manics))
- Don't run tests on unsupported k8s client versions [#464](https://github.com/jupyterhub/kubespawner/pull/464) ([@yuvipanda](https://github.com/yuvipanda))
- Migrate from travis to GitHub actions [#459](https://github.com/jupyterhub/kubespawner/pull/459) ([@consideRatio](https://github.com/consideRatio))
- Cleanup JS patch of JupyterHub 0.8 HTML not needed in 0.9+ [#455](https://github.com/jupyterhub/kubespawner/pull/455) ([@consideRatio](https://github.com/consideRatio))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2020-10-23&to=2020-12-15&type=c))

[@athornton](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aathornton+updated%3A2020-10-23..2020-12-15&type=Issues) | [@betatim](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Abetatim+updated%3A2020-10-23..2020-12-15&type=Issues) | [@captnbp](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Acaptnbp+updated%3A2020-10-23..2020-12-15&type=Issues) | [@celine168](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aceline168+updated%3A2020-10-23..2020-12-15&type=Issues) | [@clkao](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aclkao+updated%3A2020-10-23..2020-12-15&type=Issues) | [@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2020-10-23..2020-12-15&type=Issues) | [@DarkmatterVale](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3ADarkmatterVale+updated%3A2020-10-23..2020-12-15&type=Issues) | [@dkipping](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Adkipping+updated%3A2020-10-23..2020-12-15&type=Issues) | [@dtaniwaki](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Adtaniwaki+updated%3A2020-10-23..2020-12-15&type=Issues) | [@erolosty](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aerolosty+updated%3A2020-10-23..2020-12-15&type=Issues) | [@gcavalcante8808](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Agcavalcante8808+updated%3A2020-10-23..2020-12-15&type=Issues) | [@gsemet](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Agsemet+updated%3A2020-10-23..2020-12-15&type=Issues) | [@gweis](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Agweis+updated%3A2020-10-23..2020-12-15&type=Issues) | [@h4gen](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ah4gen+updated%3A2020-10-23..2020-12-15&type=Issues) | [@joelpfaff](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ajoelpfaff+updated%3A2020-10-23..2020-12-15&type=Issues) | [@manics](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Amanics+updated%3A2020-10-23..2020-12-15&type=Issues) | [@meeseeksmachine](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ameeseeksmachine+updated%3A2020-10-23..2020-12-15&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aminrk+updated%3A2020-10-23..2020-12-15&type=Issues) | [@ondave](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aondave+updated%3A2020-10-23..2020-12-15&type=Issues) | [@ryanlovett](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aryanlovett+updated%3A2020-10-23..2020-12-15&type=Issues) | [@stefanvangastel](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Astefanvangastel+updated%3A2020-10-23..2020-12-15&type=Issues) | [@support](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Asupport+updated%3A2020-10-23..2020-12-15&type=Issues) | [@tjcrone](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Atjcrone+updated%3A2020-10-23..2020-12-15&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Awelcome+updated%3A2020-10-23..2020-12-15&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2020-10-23..2020-12-15&type=Issues)

## 0.14

### [0.14.1] - 2020-10-23

#### Bugs fixed

- KubeSpawner.image_pull_secrets malfunctions in 0.14.0 - this fixes it [#451](https://github.com/jupyterhub/kubespawner/pull/451) ([@johnhoman](https://github.com/johnhoman))

#### Maintenance and upkeep improvements

- CI: bump to kubernetes client v12, and test k8s 1.19 also [#449](https://github.com/jupyterhub/kubespawner/pull/449) ([@consideRatio](https://github.com/consideRatio))

#### Contributors to this release

([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2020-10-05&to=2020-10-23&type=c))

[@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2020-10-05..2020-10-23&type=Issues) | [@johnhoman](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ajohnhoman+updated%3A2020-10-05..2020-10-23&type=Issues) | [@rkdarst](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Arkdarst+updated%3A2020-10-05..2020-10-23&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Awelcome+updated%3A2020-10-05..2020-10-23&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2020-10-05..2020-10-23&type=Issues)

### [0.14.0] - 2020-10-05

#### Enhancements made

- Allow image_pull_secrets config to be specified the k8s native way [#442](https://github.com/jupyterhub/kubespawner/pull/442) ([@consideRatio](https://github.com/consideRatio))

#### Bugs fixed

- Access containerStatuses key with get() [#441](https://github.com/jupyterhub/kubespawner/pull/441) ([@rmoe](https://github.com/rmoe))
- Allow pod to spawn if the PVC specified already exists [#438](https://github.com/jupyterhub/kubespawner/pull/438) ([@gravenimage](https://github.com/gravenimage))
- Add timeout and retry to create_namespaced_pod [#433](https://github.com/jupyterhub/kubespawner/pull/433) ([@gravenimage](https://github.com/gravenimage))
- Fix KubeIngressProxy.get_all_routes for 0.13 [#430](https://github.com/jupyterhub/kubespawner/pull/430) ([@remche](https://github.com/remche))

#### Maintenance and upkeep improvements

- Manage regexp syntax deprecation [#445](https://github.com/jupyterhub/kubespawner/pull/445) ([@consideRatio](https://github.com/consideRatio))
- Python 3.6+ migration: async in 3.5 and async with yeild in 3.6 [#444](https://github.com/jupyterhub/kubespawner/pull/444) ([@consideRatio](https://github.com/consideRatio))
- Add an explicit dependency on urllib3 [#437](https://github.com/jupyterhub/kubespawner/pull/437) ([@yuvipanda](https://github.com/yuvipanda))
- Delete remnant now unused parts in spawner.py [#382](https://github.com/jupyterhub/kubespawner/pull/382) ([@bitnik](https://github.com/bitnik))

## 0.13

### [0.13.0] - 2020-09-20

Noteworthy for this release are: performance improvements, Kubernetes native environment variable specification, the possibility to run multiple JupyterHub's in the same namespace.

#### Breaking changes

The following changes probably won't break typical usage of KubeSpawner, but could for example break logic to customized the progress page JupyerHub displays while spawning a Kubernetes pod for the user.

- The Kubernetes EventsReflector, which is providing the KubeSpawner instances with information about [Kubernetes Events](https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.19/#event-v1-core) describing events for other resources, is now exposing events as python dictionaries rather than `V1Event` objects. `V1Event` is defined in the [kubernetes-client/python](https://github.com/jupyterhub/kubespawner) library as a representation of a Kubernetes Event.
- KubeSpawner's `.progress` method implementation (https://github.com/jupyterhub/jupyterhub/pull/1771) which is generating a formatted `message` as well as a KubeSpawner specific `raw_event` entry now returns the `raw_event` as a Python dictionary with entries formatted in `camelCase` where the keys were formatted in `snake_case`.

#### New

- Support EnvVar's with 'valueFrom' as well as with 'value' [#426](https://github.com/jupyterhub/kubespawner/pull/426) ([@consideRatio](https://github.com/consideRatio))
- Breaking change / performance: don't make kubernetes-client deserialize k8s events into objects [#424](https://github.com/jupyterhub/kubespawner/pull/424) ([@rmoe](https://github.com/rmoe))
- Add component_label property to support multiple hub instances in the… [#418](https://github.com/jupyterhub/kubespawner/pull/418) ([@harsimranmaan](https://github.com/harsimranmaan))

#### Fixes

- Breaking change / performance: don't make kubernetes-client deserialize k8s events into objects [#424](https://github.com/jupyterhub/kubespawner/pull/424) ([@rmoe](https://github.com/rmoe))

#### Maintenance

- Log thread pool worker count on init [#420](https://github.com/jupyterhub/kubespawner/pull/420) ([@mriedem](https://github.com/mriedem))
- CI: test k8s 1.18 and require success, publish without test, bump minikube [#417](https://github.com/jupyterhub/kubespawner/pull/417) ([@consideRatio](https://github.com/consideRatio))

#### Contributors to this release

[@abinet](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aabinet+updated%3A2020-07-17..2020-09-03&type=Issues) | [@chancez](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Achancez+updated%3A2020-07-17..2020-09-03&type=Issues) | [@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2020-07-17..2020-09-03&type=Issues) | [@harsimranmaan](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Aharsimranmaan+updated%3A2020-07-17..2020-09-03&type=Issues) | [@meeseeksmachine](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ameeseeksmachine+updated%3A2020-07-17..2020-09-03&type=Issues) | [@mriedem](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Amriedem+updated%3A2020-07-17..2020-09-03&type=Issues) | [@rmoe](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Armoe+updated%3A2020-07-17..2020-09-03&type=Issues) | [@shenghu](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ashenghu+updated%3A2020-07-17..2020-09-03&type=Issues) | [@welcome](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Awelcome+updated%3A2020-07-17..2020-09-03&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2020-07-17..2020-09-03&type=Issues) | [@zlanyi](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Azlanyi+updated%3A2020-07-17..2020-09-03&type=Issues)

This list of contributors were generated by [`github-activity`](https://github.com/executablebooks/github-activity) according to [these criteria](https://github-activity.readthedocs.io/en/latest/#how-does-this-tool-define-contributions-in-the-reports).

## 0.12

### [0.12.0] - 2020-07-17

#### Security

- Security fix: CVE-2020-15110 / GHSA-v7m9-9497-p9gr.
  When named-servers are enabled,
  certain username patterns, depending on authenticator,
  could allow collisions.
  The default named-server template is changed to prevent collisions,
  meaning that upgrading will lose associations of
  named-servers with their PVCs if the default templates are used.
  Data should not be lost (old PVCs will be ignored, not deleted),
  but will need manual migration to new PVCs prior to deletion of old PVCs.

#### New features

- Add `slugs` field for selecting profiles in API, instead of indices. [#401](https://github.com/jupyterhub/kubespawner/pull/401) ([@stv0g](https://github.com/stv0g))
- Expose `__version__` in kubespawner module [#383](https://github.com/jupyterhub/kubespawner/pull/383) ([@consideRatio](https://github.com/consideRatio))
- log a warning if unrecognized user_options are provided [#389](https://github.com/jupyterhub/kubespawner/pull/389) ([@minrk](https://github.com/minrk))

#### Fixes

- Fix ingress compatibility with kubernetes >= 0.10.
  kubernetes >= 0.10 is now required. [#402](https://github.com/jupyterhub/kubespawner/pull/402) ([@BertR](https://github.com/BertR))
- Fix progress serialization [#381](https://github.com/jupyterhub/kubespawner/pull/381) ([@consideRatio](https://github.com/consideRatio))
- Typos in storage capacity [#384](https://github.com/jupyterhub/kubespawner/pull/384) ([@TkTech](https://github.com/TkTech))
- Typos in profile_list help [#411](https://github.com/jupyterhub/kubespawner/pull/411) ([@mriedem](https://github.com/mriedem))

#### Maintenance

- Fix CI builds [#394](https://github.com/jupyterhub/kubespawner/pull/394) ([@consideRatio](https://github.com/consideRatio))
- use bump2version and add release documentation [#376](https://github.com/jupyterhub/kubespawner/pull/376) ([@consideRatio](https://github.com/consideRatio))
- improve development documentation [#377](https://github.com/jupyterhub/kubespawner/pull/377) ([@consideRatio](https://github.com/consideRatio))
- test with JupyterHub master [#380](https://github.com/jupyterhub/kubespawner/pull/380) ([@consideRatio](https://github.com/consideRatio))
- update contributing guide [#391](https://github.com/jupyterhub/kubespawner/pull/391) ([@betatim](https://github.com/betatim))

## 0.11

### [0.11.1] - 2019-11-29

0.11.1 consists of a small bugfix that made the progress reporting break.

#### Fixes

- Fix spawn progress events now showing up due to failure to serialize [#381](https://github.com/jupyterhub/kubespawner/pull/381) ([@consideRatio](https://github.com/consideRatio))

#### Maintenance

- Don't require deploy job to also run tests [#379](https://github.com/jupyterhub/kubespawner/pull/379) ([@consideRatio](https://github.com/consideRatio))

### [0.11.0] - 2019-11-28

0.11.0 features minor feature additions, compatebility measures, and fixes.
KubeSpawner now require Python 3.5 and is no longer actively tested against
Kubernetes clusters versioned 1.10 as before, but is now being tested against
version 1.12-1.16 with the [python kubernetes client
library](https://github.com/kubernetes-client/python) version 8-11 that is
compatible with k8s 1.11-1.15.

#### New

- Add `KubeSpawner.storage_selector` for matching persistent volume using storage selector. [#338](https://github.com/jupyterhub/kubespawner/pull/338) ([@GrahamDumpleton](https://github.com/GrahamDumpleton))
- Provide `raw_event` in spawner progress [#361](https://github.com/jupyterhub/kubespawner/pull/361) ([@clkao](https://github.com/clkao))
- Add `{username}` expansion to extra_pod_config [#321](https://github.com/jupyterhub/kubespawner/pull/321) ([@cgiraldo](https://github.com/cgiraldo))
- Configurable `delete_grace_period` [#310](https://github.com/jupyterhub/kubespawner/pull/310) ([@arturozv](https://github.com/arturozv))

#### Fixes

- Scope security context to container from pod where it is possible [#334](https://github.com/jupyterhub/kubespawner/pull/334) ([@shoelsch](https://github.com/shoelsch))
- Permit storage class to be empty string. [#337](https://github.com/jupyterhub/kubespawner/pull/337) ([@GrahamDumpleton](https://github.com/GrahamDumpleton))
- Fix pod name prefix escaping for named servers [#309](https://github.com/jupyterhub/kubespawner/pull/309) ([@dmarth](https://github.com/dmarth))
- Always load user_options [#301](https://github.com/jupyterhub/kubespawner/pull/301) ([@minrk](https://github.com/minrk))
- using user_options in kubespawner [#285](https://github.com/jupyterhub/kubespawner/pull/285) ([@hhuuggoo](https://github.com/hhuuggoo))
- Allow None on UID and GID [#286](https://github.com/jupyterhub/kubespawner/pull/286) ([@dtaniwaki](https://github.com/dtaniwaki))

#### Compatibility

- CI reworked, support modern k8s high resolution timestamps, event monitoring is made more reliable, kubernetes=>8 required, python>=3.6 required, inline docs added [#368](https://github.com/jupyterhub/kubespawner/pull/368) ([@consideRatio](https://github.com/consideRatio))
- Fix for Kubernetes 1.16 regarding datetime comparison [#362](https://github.com/jupyterhub/kubespawner/pull/362) ([@consideRatio](https://github.com/consideRatio))
- More idiomatic python syntax [#356](https://github.com/jupyterhub/kubespawner/pull/356) ([@AnotherCodeArtist](https://github.com/AnotherCodeArtist))
- Compatibility with kubernetes, jupyterhub prereleases [#314](https://github.com/jupyterhub/kubespawner/pull/314) ([@minrk](https://github.com/minrk))
- compatibility with kubernetes 9.0 [#294](https://github.com/jupyterhub/kubespawner/pull/294) ([@minrk](https://github.com/minrk))
- Pin kubernetes version to 8.0 [#292](https://github.com/jupyterhub/kubespawner/pull/292) ([@yuvipanda](https://github.com/yuvipanda))

#### Maintenance

- Iteration of local development instructions [#377](https://github.com/jupyterhub/kubespawner/pull/377) ([@consideRatio](https://github.com/consideRatio))
- Add RELEASE.md and utilize bump2version [#376](https://github.com/jupyterhub/kubespawner/pull/376) ([@consideRatio](https://github.com/consideRatio))
- Fix docs build [#371](https://github.com/jupyterhub/kubespawner/pull/371) ([@consideRatio](https://github.com/consideRatio))
- [MRG]: Travis pypi: only use pre for nightly [#369](https://github.com/jupyterhub/kubespawner/pull/369) ([@manics](https://github.com/manics))
- Add relevant badges to README.md [#365](https://github.com/jupyterhub/kubespawner/pull/365) ([@consideRatio](https://github.com/consideRatio))
- Update SETUP.md instructions to match current state of JupyterHub [#353](https://github.com/jupyterhub/kubespawner/pull/353) ([@yuvipanda](https://github.com/yuvipanda))
- codecov badge [#312](https://github.com/jupyterhub/kubespawner/pull/312) ([@choldgraf](https://github.com/choldgraf))
- Update documentation regarding run_as_gid behavior [#297](https://github.com/jupyterhub/kubespawner/pull/297) ([@kevin-bates](https://github.com/kevin-bates))
- build docs with python 3.6 [#295](https://github.com/jupyterhub/kubespawner/pull/295) ([@minrk](https://github.com/minrk))
- making kubespawner docs links more discoverable [#287](https://github.com/jupyterhub/kubespawner/pull/287) ([@choldgraf](https://github.com/choldgraf))

## 0.10

### [0.10.1] - 2018-12-11

0.10.1 is a tiny bugfix release, fixing regressions in 0.10.0.

- Fix deprecation of `KubeSpawner.hub_connect_ip`,
  which caused errors in 0.10 when the deprecated config was used.

### [0.10.0] - 2018-12-05

0.10.0 is a small release, with minor changes and fixes.

- Deprecate `KubeSpawner.image_spec` configuration in favor of standard `KubeSpawner.image`. `image_spec` continues to work with deprecation warnings
- Stop pinning an exact kubernetes client version;
  instead, require kubernetes client >= 7.
  If desired, pinning should be done in images/installations
- Expand username template variables in extra_containers
- Set pod restart policy to OnFailure, so that notebook servers that terminate themselves cleanly do not restart automatically
- Formally deprecate `KubeSpawner.hub_connect_ip` and `KubeSpawner.hub_connect_ip`
  in favor of `JupyterHub.hub_connect_ip`,
  available in jupyterhub >= 0.8

## 0.9

### [0.9.0] - 2018-09-03

KubeSpawner 0.9.0 is a big release of KubeSpawner.

Change highlights:

- Require Kubernetes >= 1.6
- Require JupyterHub >= 0.8
- Require Python >= 3.5
- Expose lots more Kubernetes options
- Support configuration profiles via :attr:`.KubeSpawner.profile_list`
- Support Kubernetes events for the progress API in JupyterHub 0.9.
- Update Kubernetes Python client to 6.0 (supporting Kubernetes 1.10 APIs)
- Numerous bugfixes

[unreleased]: https://github.com/jupyterhub/kubespawner/compare/4.0.0...HEAD
[4.0.0]: https://github.com/jupyterhub/kubespawner/compare/3.0.2...4.0.0
[3.0.2]: https://github.com/jupyterhub/kubespawner/compare/3.0.1...3.0.2
[3.0.1]: https://github.com/jupyterhub/kubespawner/compare/3.0.0...3.0.1
[3.0.0]: https://github.com/jupyterhub/kubespawner/compare/2.0.1...3.0.0
[2.0.1]: https://github.com/jupyterhub/kubespawner/compare/2.0.0...2.0.1
[2.0.0]: https://github.com/jupyterhub/kubespawner/compare/1.1.2...2.0.0
[1.1.2]: https://github.com/jupyterhub/kubespawner/compare/1.1.1...1.1.2
[1.1.1]: https://github.com/jupyterhub/kubespawner/compare/1.1.0...1.1.1
[1.1.0]: https://github.com/jupyterhub/kubespawner/compare/1.0.0...1.1.0
[1.0.0]: https://github.com/jupyterhub/kubespawner/compare/0.16.1...1.0.0
[0.16.1]: https://github.com/jupyterhub/kubespawner/compare/0.16.0...0.16.1
[0.16.0]: https://github.com/jupyterhub/kubespawner/compare/0.15.0...0.16.0
[0.15.0]: https://github.com/jupyterhub/kubespawner/compare/0.14.1...0.15.0
[0.14.1]: https://github.com/jupyterhub/kubespawner/compare/0.14.0...0.14.1
[0.14.0]: https://github.com/jupyterhub/kubespawner/compare/0.13.0...0.14.0
[0.13.0]: https://github.com/jupyterhub/kubespawner/compare/0.12.0...0.13.0
[0.12.0]: https://github.com/jupyterhub/kubespawner/compare/0.10.1...0.12.0
[0.10.1]: https://github.com/jupyterhub/kubespawner/compare/0.10.0...0.10.1
[0.10.0]: https://github.com/jupyterhub/kubespawner/compare/0.9.0...0.10.0
[0.9.0]: https://github.com/jupyterhub/kubespawner/compare/v0.8.1...0.9.0
