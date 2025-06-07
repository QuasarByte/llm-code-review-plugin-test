# llm-code-review-plugin-test

This is a sample Maven project designed to **demonstrate and test the integration of the [llm-code-review-maven-plugin](https://github.com/QuasarByte/llm-code-review-maven-plugin)**.

The project contains a simple Java class and minimal configuration, providing a quick way to try out LLM-powered automated code review within a real Maven build.

---

## Project Structure
src/main/java/com/quasarbyte/llmcodereview/Main.java # Example Java source file
pom.xml # Maven configuration, plugin setup

---

## How to Use

1. **Clone this repository** or copy the `pom.xml` configuration to your own test project.

2. **Check plugin configuration** in `pom.xml`:

    - The plugin should be declared under `<build><plugins>`.
    - By default, it is configured to use the `baseUrl` property for your LLM provider.
    - You can change the LLM provider endpoint and other parameters as needed.

3. **Build and run code review:**

    ```sh
    mvn clean install
    mvn llm-code-review:llm-code-review
    ```

   The review will be performed on the example Java code.  
   Results, review comments, warnings, and statistics will be shown in your Maven output.

4. **Modify and experiment:**

    - Add more Java files to `src/main/java/` to expand the test.
    - Change plugin parameters in `pom.xml` to try different models, prompts, rules, or LLM providers.
    - Use the plugin as a reference for integrating code review automation into your real projects.

---

## Requirements

- **Java 8** or newer
- **Maven**
- Network access to your selected LLM provider (or local LLM server)

---

## License

This project is provided under the [Apache License 2.0](./LICENSE).

---

## Support

For questions, plugin issues, or feedback, see the plugin repository or contact the maintainer.

---

*This repository is for demonstration and testing purposes only.*
