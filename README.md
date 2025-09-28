# EKL Language Project

The EKL Language Project is a configuration environment language similar to JSON/YAML, written in Java. It aims to provide a flexible and powerful way to define and manage configuration settings for various applications and environments.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Simple Syntax**: EKL uses a straightforward syntax that is easy to read and write.
- **Flexible Configuration**: Supports complex configurations with nested structures.
- **Java Integration**: Seamlessly integrates with Java applications.
- **Validation**: Built-in validation to ensure configuration correctness.

## Installation

To get started with EKL, follow these steps:

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/skygenesisenterprise/ekl.git
    cd ekl
    ```

2. **Build the Project**:
    ```sh
    mvn clean install
    ```

3. **Run the Application**:
    ```sh
    java -jar target/ekl.jar
    ```

## Usage

Here is a simple example of how to use EKL in your Java application:

```java
import com.ekl.language.EKLParser;
import com.ekl.language.EKLConfig;

public class Main {
    public static void main(String[] args) {
        EKLParser parser = new EKLParser();
        EKLConfig config = parser.parse("config.ekl");

        System.out.println("Configuration loaded: " + config.toString());
    }
}
```

## Contributing

We welcome contributions from the community! To contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a new Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
