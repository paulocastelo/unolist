# 🧪 UnoList Lab — Laboratório de Testes

Este diretório contém o **laboratório de testes manuais e exploratórios** do projeto **UnoList**.

O objetivo deste ambiente é permitir que os desenvolvedores:

- ✅ Validem os serviços do back-end local.
- ✅ Realizem testes de CRUD, Queries e Backup/Restore.
- ✅ Executem testes organizados, modulares e reaproveitáveis.
- ✅ Mantenham o `main.dart` limpo e focado na aplicação real.

---

## 🏗️ Estrutura do `/lab/`

```

lab/
├── crud\_tests/          # Testes de CRUD (Create, Read, Update, Delete)
│   ├── category\_crud\_test.dart
│   └── task\_crud\_test.dart
├── backup\_tests/        # Testes de Backup e Restore
│   └── backup\_test.dart
├── query\_tests/         # Testes de filtros e buscas
│   └── task\_query\_test.dart
├── lab\_main.dart        # 🚀 Arquivo principal que executa todos os testes sequencialmente
└── README.md            # Este arquivo de documentação

````

---

## 🚀 Como executar o UnoList Lab

No terminal:

```bash
flutter run -t lib/lab/lab_main.dart
````

Ou no Android Studio:

1. Clique com o botão direito no arquivo **`lab_main.dart`**.
2. Selecione **"Run 'lab\_main.dart'"**.

---

## 🔥 Fluxo de execução

O arquivo **`lab_main.dart`** executa os testes de forma **sequencial e automática**, na seguinte ordem:

1️⃣ **CRUD de Categorias**
2️⃣ **CRUD de Tarefas**
3️⃣ **Consultas (Queries) de Tarefas**
4️⃣ **Backup e Restore**

Todos os testes são rodados em sequência, e os resultados são exibidos no console.

---

## 🧠 Descrição dos Testes

| Diretório       | Arquivo                   | Descrição                                                          |
| --------------- | ------------------------- | ------------------------------------------------------------------ |
| `crud_tests/`   | `category_crud_test.dart` | Testes de criação, listagem, atualização e exclusão de categorias. |
|                 | `task_crud_test.dart`     | Testes de CRUD completo para tarefas.                              |
| `backup_tests/` | `backup_test.dart`        | Teste de exportação e importação de backup JSON.                   |
| `query_tests/`  | `task_query_test.dart`    | Testes de filtros de tarefas (status, categoria).                  |
| 🔗 Raiz         | `lab_main.dart`           | Arquivo principal que executa todos os testes sequencialmente.     |

---

## 💎 Vantagens deste Lab

* 🔥 Ambiente seguro para testar sem afetar o app real.
* 🏗️ Arquitetura limpa, modular e escalável.
* 🧠 Serve como documentação viva do funcionamento dos serviços do back-end.
* ✅ Facilita debugging, desenvolvimento e validação de novas features.

---

## 🧠 Boas práticas recomendadas

* 🔸 Crie novos subdiretórios caso precise de mais categorias de testes (`performance_tests/`, `stress_tests/`, `integration_tests/`, etc.).
* 🔸 Sempre mantenha os testes no Lab separados do app principal.
* 🔸 O Lab não deve ser incluído no build de produção.

---

## 🚫 Atenção

> Este diretório é **exclusivo para desenvolvimento interno**.
> **Não deve ser incluído em builds de produção ou distribuição do app final.**

---

## ✨ Autor

**Paulo Castelo** – *aka* **ZeroAvenger**
🔗 [LinkedIn](https://www.linkedin.com/in/paulo-castelo/) | 🚀 [GitHub](https://github.com/paulocastelo)

---

## 📜 Licença

Este projeto está licenciado sob a [MIT License](../../LICENSE).

```
