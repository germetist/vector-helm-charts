# Changelog
All notable changes to this project will be documented in this file.

This project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)

## [vector-0.15.1] - 2022-08-11

### Vector

#### Bug Fixes

- Bump to Vector v0.23.3 (#234) ([fae2f7a](https://github.com/vectordotdev/helm-charts/commit/fae2f7a70fc749d7d917caf946b311f8ac52da35))

## [vector-0.15.0] - 2022-08-10

### Vector

#### Features

- Add lifecycle ([2dc5602](https://github.com/vectordotdev/helm-charts/commit/2dc560265d9008157ce7389f1147a21f9d1fbeef))

## [vector-0.14.0] - 2022-07-11

### Vector

#### Features

- Bump Vector to 0.23.0 ([ba2fcd8](https://github.com/vectordotdev/helm-charts/commit/ba2fcd8fb6f918b8b853de45a8e43fea777e1295))

## [vector-0.13.2] - 2022-06-30

### Vector

#### Bug Fixes

- Bump Vector version to 0.22.3 ([3177be3](https://github.com/vectordotdev/helm-charts/commit/3177be318994dd2d4d8ce466e723d13266f1f271))

#### Features

- Allow enabling of collection vector container logs by vector (#222) ([a4e9b7a](https://github.com/vectordotdev/helm-charts/commit/a4e9b7adcf780928fb0a4f5f989c760f75e53d9d))

## [vector-0.13.1] - 2022-06-17

### Vector

#### Bug Fixes

- Bump Vector version v0.22.2 ([b91a76e](https://github.com/vectordotdev/helm-charts/commit/b91a76ec4ee78123597f66886012fbfece2ba382))

## [vector-0.13.0] - 2022-06-13

### Vector

#### Features

- Add digest option to vector image ([6e54a0a](https://github.com/vectordotdev/helm-charts/commit/6e54a0a463c47ec57e5f8b315e40a07ae584b878))

## [vector-0.12.0] - 2022-06-01

### Vector

#### Features

- Bump chart appVersion to 0.22.0 ([a6eb7fc](https://github.com/vectordotdev/helm-charts/commit/a6eb7fcdfceb981f9d133519fbc191f8f281045f))

## [vector-0.11.0] - 2022-05-20

### Vector

#### Features

- Add ability to list and watch nodes ([081fa33](https://github.com/vectordotdev/helm-charts/commit/081fa33118f63cfde6e6cae0c0e1a430e53948eb))

## [vector-0.10.3] - 2022-05-06

### Vector

#### Bug Fixes

- Bump to Vector 0.21.2 ([7150a1b](https://github.com/vectordotdev/helm-charts/commit/7150a1b56fd06f275d8fc0632469e9837ad26838))

## [vector-0.10.2] - 2022-04-27

### Vector

#### Bug Fixes

- No need to set replicas to Statefulset when using autoscaling ([9d4fdb3](https://github.com/vectordotdev/helm-charts/pull/203/commits/7d01231b484f080df31efda465dc0cb1b31262b5))

## [vector-0.10.1] - 2022-04-22

### Vector

#### Bug Fixes

- Bump image to 0.21.1 ([9d4fdb3](https://github.com/vectordotdev/helm-charts/commit/9d4fdb3fb89262d5f30f908abae70472e00b92f8))

## [vector-0.10.0] - 2022-04-14

### Vector

#### Features

- Switch policy version based on capabilities and k8s version (#197) ([347403e](https://github.com/vectordotdev/helm-charts/commit/347403e4ad810ccde77f2927b675ed04b6a2f322))
- Bump image to 0.21.0 ([28f48bd](https://github.com/vectordotdev/helm-charts/commit/28f48bd0577109395ccffad279e6d81a72bab1de))

## [vector-0.9.0] - 2022-04-12

### Vector

#### Bug Fixes

- Bump Vector to v0.20.1 ([8a03f17](https://github.com/vectordotdev/helm-charts/commit/8a03f1728c1007b02e8ad6e029a41bb01d1f2d8d))

#### Documentation

- Add quickstart values and docs (#176) ([ce17ab6](https://github.com/vectordotdev/helm-charts/commit/ce17ab665824768634fa1cab0c31d8b3b3e97b0e))

#### Features

- Improve help text printed by NOTES.txt and reduce duplication of internal templates (#189) ([e5d994c](https://github.com/vectordotdev/helm-charts/commit/e5d994c84a74be029061c55caa986d913b2f060a))
- Add help output for configurations with datadog_agent source (#178) ([13aadfb](https://github.com/vectordotdev/helm-charts/commit/13aadfb10163fa7c36698acd9a492b4023d73a7b))

## [vector-0.7.0] - 2022-03-23

### Vector

#### Bug Fixes

- Update app.kubernetes.io/version to be the image.tag if it is set. (#179) ([782a50a](https://github.com/vectordotdev/helm-charts/commit/782a50aebf7bbd4d73ca06dccd8a704b5e561b9b))
- Fix conditionals for existingConfigMaps and haproxy.existingConfigMap (#182) ([87ca537](https://github.com/vectordotdev/helm-charts/commit/87ca537b54f9956c434ddbbd3cfcc9942d7e9c07))
  - **BREAKING**: Several templates were referencing a previously removed `existingConfig`, they've been updated to use either `existingConfigMaps` or `haproxy.existingConfigMap`
- Use haproxy.image.tag as its version label value (#183) ([3983653](https://github.com/vectordotdev/helm-charts/commit/39836533d6f8c41c07ddb341641e0fe328537234))
  - **BREAKING**: Labels on HAProxy resources were being passed the `AppVersion` value, leading them to be labeled with Vector's version rather than HAProxy's version

#### Documentation

- Update comment for autoscaling.enabled (#169) ([d226dd2](https://github.com/vectordotdev/helm-charts/commit/d226dd224eef9e2e598a62702162d774562778ed))

#### Features

- Add list verb for upcoming kube-rs change (#166) ([068af80](https://github.com/vectordotdev/helm-charts/commit/068af80e688214ca84325717e4c13e09830c765c))

## [vector-0.7.0-rc.0] - 2022-03-08

### Vector

#### Features

- Add list verb for upcoming kube-rs change ([e390ead](https://github.com/vectordotdev/helm-charts/commit/e390ead62dcc5e2736d9fb7cb1f19ac7684f3d92))

## [vector-0.6.0] - 2022-02-11

### Vector

#### Features

- Update to use 0.20.0 (#164) ([e0f7573](https://github.com/vectordotdev/helm-charts/commit/e0f7573eb84ec2000b4601540076733d93b6148a))

## [vector-0.5.2] - 2022-02-11

## [vector-0.5.1] - 2022-02-09

### Vector

#### Documentation

- Update maintainer email (#161) ([a3dc59a])(https://github.com/vectordotdev/helm-charts/commit/a3dc59aaeaa36bd9f25c527023dbad394e0d3c58)

## [vector-0.5.0] - 2022-02-07

### Vector

#### Bug Fixes

- Include common labels on ClusterRole resource (#144) ([01773ba](https://github.com/vectordotdev/helm-charts/commit/01773baf98257c056f42793bb5f4c136a2926d2a))

#### Documentation

- Fix comment on autoscaling option (#145) ([9d1c3c2](https://github.com/vectordotdev/helm-charts/commit/9d1c3c29575c14b8d2d1a85fe611332d96816d18))
- Fix loki label ends with new line (#154) ([e59c63b](https://github.com/vectordotdev/helm-charts/commit/e59c63be55aa0712aa6b9a35e3c5901d27593770))

#### Features

- Add honorLabels and honorTimestamps to PodMonitor (#153) ([5a92272](https://github.com/vectordotdev/helm-charts/commit/5a9227209d33efc513f5e282d076d8df438205c6))
- Upgrade Vector to 0.19.1 (#157) ([be0dc41](https://github.com/vectordotdev/helm-charts/commit/be0dc411693bd2001b443a1545d9fb810403feeb))

## [vector-0.4.0] - 2022-01-12

### Vector

#### Bug Fixes

- Include common labels on ClusterRole resource (#144) ([01773ba](https://github.com/vectordotdev/helm-charts/commit/01773baf98257c056f42793bb5f4c136a2926d2a))

#### Documentation

- Fix comment on autoscaling option (#145) ([9d1c3c2](https://github.com/vectordotdev/helm-charts/commit/9d1c3c29575c14b8d2d1a85fe611332d96816d18))

## [vector-0.3.0] - 2021-12-28

### Vector

#### Documentation

- Fix example and CI for Vector templating (#126) ([e28ba32](https://github.com/vectordotdev/helm-charts/commit/e28ba3284089d26359d7ea7e87918dc5b9b33257))
- Clarify usage of secrets.generic and env (#129) ([1396dd4](https://github.com/vectordotdev/helm-charts/commit/1396dd42309c8aeded6d20be2a2cc2b9c4e26d1b))

#### Features

- Update charts to Vector 0.19.0 (#131) ([26f9779](https://github.com/vectordotdev/helm-charts/commit/26f9779f49dfc67d76c6b33cfd126f2458a8dc20))

### Vector-aggregator

#### Bug Fixes

- Fix the conditions for enable/disable SA on the HAProxy (#122) ([83cf509](https://github.com/vectordotdev/helm-charts/commit/83cf5091825fbff872819251e00808befc41a331))

## [vector-0.2.2] - 2021-11-30

### Vector

#### Features

- Upgrade Vector to 0.18.1. (#124) ([20f1f0e](https://github.com/vectordotdev/helm-charts/commit/20f1f0e91ac9142d958f112022c9448b62cd46ce))

## [vector-0.2.1] - 2021-11-23

### Vector

#### Bug Fixes

- Switch metric list order in HPA. (#117) ([0a214bb](https://github.com/vectordotdev/helm-charts/commit/0a214bb9f49cf35d4c7d891becdecf84433b9e25))
- Typo podPriorityClassName & StatefulSet (#116) ([31d7eb4](https://github.com/vectordotdev/helm-charts/commit/31d7eb4154fc7ebd81573d6dcbf6de35cd303771))

## [vector-0.2.0] - 2021-11-19

### Vector

#### Features

- Include option to add additionalLabels to PodMonitor (#111) ([0a71e9e](https://github.com/vectordotdev/helm-charts/commit/0a71e9e653431c02ac0273e0b5556fbf1e5e8ded))
- Upgrade Vector to 0.18.0 (#114) ([27b9e98](https://github.com/vectordotdev/helm-charts/commit/27b9e9804a26893a84a46affa69b6f6738ba3b31))

## [vector-0.1.1] - 2021-11-10

### Vector

#### Documentation

- Handle helm-docs processing of vector template example (#107) ([34cb0eb](https://github.com/vectordotdev/helm-charts/commit/34cb0ebeecde276b67ee943a7559543434508930))

## [vector-0.1.0] - 2021-11-09

### Vector

#### Bug Fixes

- Provide default value for only minAvailable in PDB (#98) ([6fcb9de](https://github.com/vectordotdev/helm-charts/commit/6fcb9de045f2c0b0b01bf99082413b7574114ed1))
- Fix type for podDisruptionBudget.maxUnavailable (#104) ([190c2b4](https://github.com/vectordotdev/helm-charts/commit/190c2b437eaea344d037622d8dc5b129e60626d2))
- Toggle both service and headless service with service.enabled (#101) ([a8b7daf](https://github.com/vectordotdev/helm-charts/commit/a8b7dafa4fc6e9bc93ca3669ece7c666a398dc88))

#### Documentation

- Add example customConfig in values.yaml (#102) ([59161b9](https://github.com/vectordotdev/helm-charts/commit/59161b94b1540699c87d18b2eb27a7f8ad4a7adc))
- Add upgrade docs (#75) ([a40bdcc](https://github.com/vectordotdev/helm-charts/commit/a40bdcc5673e7bfe295bcf80690dbc73d6221f43))

## [vector-0.1.0-beta.2] - 2021-11-02

### Vector

#### Bug Fixes

- Upgrade chart to 0.17.3 ([3cf1df5](https://github.com/vectordotdev/helm-charts/commit/3cf1df50ddd16a0db13924c4412fef8d5cc0ffef))
- Fix vector proto in haproxy config (#94) ([b0a7d7d](https://github.com/vectordotdev/helm-charts/commit/b0a7d7d6e430c93376e498ce1653ac9a331d5e60))

#### Documentation

- Document how to use Vector's template syntax in customConfig (#91) ([cf67558](https://github.com/vectordotdev/helm-charts/commit/cf675581854210d128160bd787e9040a96809538))

#### Features

- Add support for user defined initContainers for Vector Pods (#79) ([44a2e5e](https://github.com/vectordotdev/helm-charts/commit/44a2e5ed0877a12a4906947926ea8d576174f006))
- Update secrets.generic to take unencoded values (#84) ([5f66c18](https://github.com/vectordotdev/helm-charts/commit/5f66c1865851894df9d682ffea688f2c95662cf7))
  - **BREAKING**: Update secrets.generic to take unencoded values (#84)
- Ensure good feature parity for HAProxy (#85) ([0cb3798](https://github.com/vectordotdev/helm-charts/commit/0cb379805e464f5dc3ba4180636ba05eefb935ca))
- Update charts to Vector 0.17.2 (#89) ([de3cf26](https://github.com/vectordotdev/helm-charts/commit/de3cf2663eee09360286c15ac8bd85a7f3a0dec2))
- Allow HPA to be used with statefulsets (#92) ([73ae867](https://github.com/vectordotdev/helm-charts/commit/73ae867c31397db64765792a87b2c67c07873919))

## [vector-0.1.0-alpha.4] - 2021-10-01

### Unscoped

#### Documentation

- Clarify suggested usage (#76) ([0555fb0](https://github.com/vectordotdev/helm-charts/commit/0555fb0d339cef1a1815203198102f6e5b0153e7))

### Vector

#### Bug Fixes

- Fix ordering of `default` function in port helpers (#80) ([bc8401f](https://github.com/vectordotdev/helm-charts/commit/bc8401fa449c70845f922c89aa5c6067ffbf23cc))

#### Features

- Add optional PodDisruptionBudget resource for Vector (#57) ([ea65bd0](https://github.com/vectordotdev/helm-charts/commit/ea65bd095cb876b29a747954fdaef28370d87a22))
- Support injecting multiple ConfigMaps (#58) ([337d7d2](https://github.com/vectordotdev/helm-charts/commit/337d7d231ee1d307987fe4945a37bfa6f44c5342))
  - **BREAKING**: Renamed `existingConfigMap` to `existingConfig` and `haproxy.existingConfigMap` to `haproxy.existingConfig`
- Allow option PSP to be created for Agent role (#67) ([a2c535b](https://github.com/vectordotdev/helm-charts/commit/a2c535be68f8fb57ab19e9f852e10312405c6a19))
- Allow for manually setting ports for container and services (#68) ([5901de8](https://github.com/vectordotdev/helm-charts/commit/5901de8e6e68aaff976105f3be59b89f06732c43))
- Create checksum annotations for existingConfig and extraConfigs (#69) ([26a1bd5](https://github.com/vectordotdev/helm-charts/commit/26a1bd52c70dc849ef69ba78f8a60dcde0092f5d))
- Consolidate existing/extraConfig options (#71) ([17c94b8](https://github.com/vectordotdev/helm-charts/commit/17c94b8cbf21e6b1f1dedf329f74f8b928be5d46))
  - **BREAKING**: Renamed existingConfig to existingConfigMaps, renamed haproxy.existingConfig to haproxy.existingConfigMaps removed extraConfigs
- Add parameter to include additional labels on all resources (#73) ([6d1426b](https://github.com/vectordotdev/helm-charts/commit/6d1426b89323d85dd6a9d698aaba550194ce21e4))
- Add extraVolumes and extraVolumeMounts parameters (#74) ([895354f](https://github.com/vectordotdev/helm-charts/commit/895354f4e3ef47a29b36d172187e350add40b535))

## [vector-0.1.0-alpha.3] - 2021-09-17

### Vector

#### Bug Fixes

- Create ports for api from customConfig (#51) ([b82c6b6](https://github.com/vectordotdev/helm-charts/commit/b82c6b62f1f73febbd5ec6ce787e829148f6ef22))

#### Features

- Add override for default Vector command (#49) ([29710f3](https://github.com/vectordotdev/helm-charts/commit/29710f33339f9a9645ffb21e045a391fc13ac335))
- Add support for topologyKeys on all Services (#50) ([47f9e2b](https://github.com/vectordotdev/helm-charts/commit/47f9e2b9ee482d073b99a353fa6d403787a935f6))
- Add optional Ingress resource (#53) ([2b87bf0](https://github.com/vectordotdev/helm-charts/commit/2b87bf01596bb7d4c2583deb4ba8d7a13cb4074f))

<!-- generated by git-cliff -->
