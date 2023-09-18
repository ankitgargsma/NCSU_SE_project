**Introduction:**

The "Units Converter" Chrome extension project presented several significant challenges while understanding and running it. This document will explore these challenges, delve into their difficulties, discuss how they could have been avoided, and outline the practices to be implemented in an improved project version to prevent such challenges.

**Challenges Faced:**

Lack of Functional Specification:

The absence of a functional specification made it arduous to understand the exact purpose and functionality of the project's features. This lack of clarity hindered our progress and forced us to deduce the functionality through trial and error.

Hardcoded Values:

Hardcoding values within the codebase proved to be a significant stumbling block. It led to incorrect results and made debugging a formidable task. Relying on hardcoded values for critical operations can result in inconsistencies and errors that are difficult to pinpoint. Also, the extension gives out values that are close to zero; for example, while converting one second to other measurements of time, we also get the conversion in the week, which is negligible.

Compatibility Issues:

The project's development on an outdated operating system caused compatibility issues when running it on modern environments. Adapting the environment to match the project's requirements consumed valuable time. Additionally, deprecated libraries within the code made finding and integrating their replacements challenging. For instance, the manifest version used is version 2, but Google depreciated the version in Jan 2023, so we have moved all our code base to version 3.

Inadequate Unit Tests:

The project's rudimentary unit tests could have covered the full range of features. Comprehensive unit testing is essential to ensure the reliability and accuracy of the product. The lack of robust testing meant many issues went undetected until the code was executed.

Misinterpretation of Units:

Running the code revealed significant bugs in functionality and results. For instance, a unit "Data Storage" was incorrectly considered "Data Transfer Speed," leading to incorrect outcomes. A clear understanding of units is crucial in a unit conversion application, and such misinterpretations can severely impact its utility. Similarly, when converting the weight from lbs to any other unit of measurement, the program will only give us an output if it's "lbs," not "lb."

3rd Party API Calls: -

The currency conversion is called a 3rd party API to get the current rate of conversions from one currency to another. Still, the API is no longer supported, leading to errors. That significant time and usage of unidentified variables make it more challenging to understand what value is returned or assigned to a variable.

Inadequate Error Handling:

The project needed better error handling, resulting in obscure error messages and frequent application crashes. Effective error handling is essential for diagnosing and resolving issues efficiently.

Complex Codebase:

The extensive and intricate nature of the codebase made it challenging to comprehend the overall architecture and flow of the application. This complexity impeded identifying and isolating specific issues, prolonging the debugging process.

Lack of Documentation:

The most critical challenge was the need for comprehensive documentation. The absence of documentation left us to decipher the project's logic, structure, and dependencies independently. This increased the learning curve and hindered progress significantly.

Unresolved Errors: -

There are a couple of unresolved errors present in the program. However, it was not hindering the output in the background, there was a list of errors like in the conversion scripts "module. exports = Currency" in giving out an issue "Uncaught ReferenceError: module is not defined," which can quickly be resolved with the help of if condition.

**Avoiding Future Challenges:**

To avoid encountering similar challenges in future projects, the following practices should be implemented:

Detailed Functional Specification:

Develop and maintain a comprehensive functional specification that defines the project's purpose, features, and functionality. This document serves as a roadmap for all stakeholders, ensuring everyone is on the same page.

Keep Libraries and Dependencies Up-to-Date:

Regularly update libraries and dependencies to prevent compatibility issues. Ensure deprecated components are replaced promptly.

Thorough Unit Testing:

Implement comprehensive unit tests that cover all project features and edge cases. Automated testing helps identify issues early in development.

Clear Unit Definitions:

Ensure a clear understanding of unit definitions within a unit conversion project to prevent misinterpretations and incorrect results.

Effective Error Handling:

Develop robust error handling mechanisms with descriptive error messages to simplify issue diagnosis and resolution.

Documentation Is Key:

Maintain thorough documentation, including code comments, README files, and user guides. Comprehensive documentation aids in project understanding and future maintenance.

**Conclusion:**

Running the "Units Converter" Chrome extension project revealed challenges from a lack of documentation, hardcoded values, compatibility issues, etc. Implementing the suggested best practices in future projects can mitigate these challenges, leading to more efficient development and enhanced project reliability.
