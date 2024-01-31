(This is what ChatGPT thinks should be the description)
# Value Insight for Bundled Items (VIBI)
**VIBI** is a tool born from a blend of personal challenge and curiosity, designed primarily for gamers who are keen on maximizing value from their game purchases. Originally inspired by the intricacies of bundle offerings in Lords Mobile, VIBI aims to be a versatile tool that can be adapted to various games where items are sold in bundles.

## Key Features:

- **Bundle Value Estimation:** Helps gamers estimate the value of individual items within game bundles, enhancing their decision-making process for purchases.
- **Customizable for Different Games:** Although inspired by Lords Mobile, VIBI is built to be flexible, allowing users to input data from different games.
- **Simple and Accessible:** Created with the gaming community in mind, the tool is straightforward and easy to use, regardless of your background.
- **Data-Driven Insights:** Empowers users to make more informed choices by providing clear insights into the value of bundled items.
- **Community Driven:** As a project born out of personal interest, VIBI values community input and suggestions for enhancements.

## Ideal for:
- Gamers looking to get the most value out of their purchases in games like Lords Mobile and others.
- Players interested in understanding the economics of game bundles and how to make strategic choices.
- Anyone curious about the value dynamics in game economies and how to apply data for better purchasing decisions.

## Getting Started:

Getting started with VIBI is easy! Just clone the repository, and you'll find straightforward instructions in the documentation on how to set it up and start using it.

## Folder Structure Explanation

This project follows the Clean Architecture principles as proposed by Jason Taylor. The structure is organised into distinct layers with specific responsibilities. Here's a guide to what each folder should contain:

### src/

#### Application
- **Behaviours**: Common CQRS pipeline behaviours (e.g., validation, logging).
- **Commands**: Command handlers and command requests.
- **Queries**: Query handlers and query requests.
- **DTOs**: Data transfer objects for exchanging data between layers.
- **Exceptions**: Custom exceptions for the application layer.
- **Interfaces**: Application layer interfaces, typically for services.
- **Mappings**: Configuration for object-object mappings.
- **Services**: Business logic services.
- **Validation**: Command and query validation rules.

#### Domain
- **Entities**: Core business entities.
- **Enums**: Enumeration types for static, named constants.
- **Events**: Domain events indicating significant occurrences.
- **Exceptions**: Custom exceptions for domain logic.
- **Interfaces**: Interfaces such as repository interfaces defined in the domain.
- **ValueObjects**: Immutable objects that are defined by their attributes.

#### Infrastructure
- **Data**: Database context, migrations, and configurations.
- **Repositories**: Implementations of domain repository interfaces.
- **Services**: Implementations of services like email, file storage.
- **Identity**: Identity and user management related classes and services.

#### WebApi
- **Controllers**: API controllers to handle HTTP requests.
- **Filters**: Filters for handling cross-cutting concerns.
- **DTOs**: Data transfer objects for API data shaping.
- **Middleware**: Custom middleware components.
- **Startup**: Configuration and services initialization.

### test/

#### Application.UnitTests
- **CommandTests**: Tests for command handlers.
- **QueryTests**: Tests for query handlers.
- **ValidatorTests**: Tests for validators.

#### Domain.UnitTests
- **EntityTests**: Tests for domain entities.
- **ValueObjectTests**: Tests for value objects.

#### Infrastructure.IntegrationTests
- **RepositoryTests**: Database interaction tests.
- **ServiceTests**: External service integration tests.

#### WebApi.IntegrationTests
- **ControllerTests**: API controller functionality tests.

Please adhere to this structure to maintain a clean and consistent codebase.

## Contributing:

VIBI is a pet project created for challenging myself to test my cloud knowledge while refreshing my coding skills. If you have ideas, bug reports, or improvements, feel free to contribute.

## License:

VIBI is released under MIT, making it freely available for everyone.

Dive into the world of smart gaming purchases with Value Insight for Bundled Items and optimize your gaming experience!
