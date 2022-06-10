# Feature Brick

A brick to create a feature using best practices and your state management of choice! Supports bloc, Provider, Riverpod, none

## How to use 🚀

```
mason make feature_brick --feature_name login --state_management bloc --use_equatable true
```

## Variables ✨

| Variable           | Description                     | Default | Type      | Conditional | When       |
| ------------------ | ------------------------------- | ------- | --------- | ----------- | ---------- |
| `feature_name`     | The name of the feature         | login   | `string`  | false       | N/A        |
| `state_management` | The state management of the app | bloc    | `enum`    | false       | N/A        |
| `use_equatable`    | Use the equatable package       | true    | `boolean` | true        | Using Bloc |

## Outputs 📦

```
--feature_name login --state_management bloc
├── login
│   ├── bloc
│   │   ├── bloc.dart
│   │   ├── login_bloc.dart
│   │   ├── login_event.dart
│   │   └── login_state.dart
│   ├── view
│   │   └── login_page.dart
│   ├── widgets
│   │   ├── login_body.dart
│   │   └── widgets.dart
│   └── login.dart
└── ...
```

```
--feature_name login --state_management provider
├── login
│   ├── provider
│   │   ├── login_provider.dart
│   │   ├── provider.dart
│   ├── view
│   │   └── login_page.dart
│   ├── widgets
│   │   ├── login_body.dart
│   │   └── widgets.dart
│   └── login.dart
└── ...
```

```
--feature_name login --state_management riverpod
├── login
│   ├── provider
│   │   ├── login_provider.dart
│   │   ├── provider.dart
│   ├── view
│   │   └── login_page.dart
│   ├── widgets
│   │   ├── login_body.dart
│   │   └── widgets.dart
│   └── login.dart
└── ...
```

```
--feature_name login --state_management none
├── login
│   ├── view
│   │   └── login_page.dart
│   ├── widgets
│   │   ├── login_body.dart
│   │   └── widgets.dart
│   └── login.dart
└── ...
```

### Roadmap

- [ ] Add Domain Layer Option
- [ ] Add Models into Domain Layer Option
- [ ] Add Services Option
- [ ] Add Ability to chose Riverpod provider type
