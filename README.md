[Android Studio](https://developer.android.com/studio) [Gradle](https://gradle.org) [JUnit](https://junit.org/junit5/)

# Android com Java - Dispositivos Móveis UTFPR

**Repositório da Pós-Graduação UTFPR**: Implementações práticas de **Activities**, **Layouts**, **Ciclo de Vida**, **Persistent Storage**, **APIs REST** e **Padrões Android**. **Gradle otimizado**, **Architecture Components** e **boas práticas de UI/UX**.

## 📱 Características do Projeto

| Recurso | Status | Detalhe |
|---------|--------|----------|
| **Activities & Fragments** | ✅ | Ciclo de vida, State Management |
| **Material Design** | ✅ | Components modernos, RecyclerView |
| **Storage Local** | ✅ | SharedPreferences, Room Database |
| **REST APIs** | ✅ | Retrofit 2, Coroutines |
| **Padrões de Projeto** | ✅ | MVC, MVVM, Repository Pattern |
| **Testes** | ✅ | Espresso, JUnit 5 |
| **Gradle Build** | ✅ | Otimizado para CI/CD |

## 🏗️ Estrutura Gradle

```
DispositivosAndroidComJavaUTFPR/
├── app/                          # Módulo principal da aplicação
│   ├── src/main/java/            # Código-fonte Java
│   │   ├── activities/           # Activities (UI Controllers)
│   │   ├── fragments/            # Fragments (UI Components)
│   │   ├── adapters/             # RecyclerView Adapters
│   │   ├── models/               # Data Models, DTOs
│   │   ├── services/             # API Services (Retrofit)
│   │   ├── database/             # Room Database, DAOs
│   │   └── utils/                # Utilities & Helpers
│   ├── src/main/res/             # Recursos (Layouts, Drawables, etc)
│   │   ├── layout/               # XML Layouts
│   │   ├── drawable/             # Imagens e ícones
│   │   └── values/               # Strings, Colors, Dimens
│   └── src/test/java/            # Testes unitários (JUnit)
├── gradle/                       # Configuração Gradle
├── build.gradle                  # Build Script principal
└── settings.gradle               # Configuração de módulos
```

## 💻 Stack Tecnológico

- **Linguagem**: Java 17+
- **Android SDK**: Min 24 | Target 35
- **Build System**: Gradle 8.x
- **Testing**: JUnit 5, Espresso
- **Architecture**: MVC/MVVM com Repository Pattern
- **Networking**: Retrofit 2 + OkHttp
- **Database**: Room ORM

## 🚀 Como Executar

### Pré-requisitos

```bash
# Certifique-se de ter instalado:
- Android Studio Arctic Fox ou superior
- JDK 17+
- Android SDK Level 24+
- Gradle 8.x
```

### Setup & Build

```bash
# Clone o repositório
git clone git@github.com:matheusBraga10/DispositivosAndroidComJavaUTFPR.git
cd DispositivosAndroidComJavaUTFPR

# Abra no Android Studio
# File > Open > Selecione a pasta

# Build do projeto
./gradlew build

# Executar testes
./gradlew test

# Instalar APK no emulador/dispositivo
./gradlew installDebug
./gradlew installRelease
```

## 📚 Conceitos Coberidos

### 1️⃣ Fundações Android

- **Android Manifest**: Permissões, Activities, Services
- **Ciclo de Vida**: onCreate(), onStart(), onResume(), onPause(), onStop(), onDestroy()
- **Context & Application**: Gerenciamento de recursos

### 2️⃣ Interface do Usuário (UI)

- **Layouts XML**: LinearLayout, ConstraintLayout, FrameLayout
- **Material Design 3**: Componentes modernos
- **RecyclerView**: Listas eficientes com Adapter Pattern
- **View Binding**: Type-safe view references

### 3️⃣ Persistência de Dados

```java
// SharedPreferences
SharedPreferences prefs = getSharedPreferences("user", MODE_PRIVATE);
prefs.edit().putString("name", "João").apply();

// Room Database
@Entity(tableName = "usuarios")
public class Usuario {
    @PrimaryKey(autoGenerate = true)
    public int id;
    public String nome;
    public String email;
}
```

## 👨‍💼 Autor

**Matheus Felipe Braga**
- GitHub: [@matheusBraga10](https://github.com/matheusBraga10)
- Email: matheusbraga10@gmail.com
- Pós-Graduação em Tecnologias Java – UTFPR
- Backend Java Developer @ PRODEMGE
- Belo Horizonte, MG | Brasil

## 📄 Licença

Este projeto está licenciado sob a **Licença MIT** - veja o arquivo [LICENSE](LICENSE) para detalhes.
