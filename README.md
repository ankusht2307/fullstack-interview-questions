# fullstack-interview-questions
Interview question for experienced fullstack individuals.

### Table of Contents

| No. | Questions                                                                                                       |
| --- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1. | [What is Test Pyramid?](#what-is-test-pyramid)

## Testing

1. ### What is Test Pyramid?

    The ***Test Pyramid*** is a concept in software testing that provides a strategy for structuring automated tests in layers to ensure ***fast, reliable, and cost-effective testing***.

    It was introduced by Mike Cohn in his book Succeeding with Agile.

    #### Structure of the Test Pyramid

    The pyramid is divided into three main layers (from bottom to top):

    1. Unit Tests (Base Layer)
        - Smallest, fastest, cheapest tests.
        - Test individual functions, classes, or components in isolation.
        - Provide quick feedback.
        - Example: testing a function that calculates discounts.

    2. Service/Integration Tests (Middle Layer)
        - Test interactions between components or services.
        - Ensure that different modules work together as expected.
        - Slower and more expensive than unit tests.
        - Example: testing whether your application correctly saves data into a database.

    3. UI/End-to-End Tests (Top Layer)
        - Test the system from the user’s perspective.
        - Cover complete workflows through the user interface or API.
        - Slowest and most brittle (high maintenance).
        - Example: automating a login test through a browser.

    #### Why Pyramid Shape?
    - Wide base (many unit tests): They are cheap, fast, and should form the majority.
    - Narrow middle (fewer integration tests): Enough to ensure modules/services connect correctly.
    - Narrow top (very few UI/E2E tests): Only for critical workflows, since they’re slow and flaky.

    #### ✅ Goal of Test Pyramid:
    - Balance speed, reliability, and coverage.
    - Catch most bugs early (with unit tests).
    - Ensure system integration works (with fewer but meaningful integration tests).
    - Validate critical user flows (with minimal end-to-end tests).

    **[⬆ Back to Top](#table-of-contents)**