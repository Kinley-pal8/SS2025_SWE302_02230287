# Practical 8 Report: GUI Testing with Cypress

**Student:** Kinley-pal8  
**Module:** SWE302 Software Engineering Methodologies  
**Date:** October 29, 2025
**GitHub Repository:** [https://github.com/Kinley-pal8/Swe302_p8](https://github.com/Kinley-pal8/Swe302_p8)

---

## Executive Summary

This report documents the implementation of comprehensive GUI testing using Cypress for Next.js web applications. The project demonstrates advanced testing methodologies including UI validation, user interaction testing, API mocking, and end-to-end user journey testing.

### Key Results

- **Test Pass Rate:** 100% (25+ test scenarios)
- **Test Files:** 8 comprehensive test files
- **Custom Commands:** 3 reusable command functions
- **Page Objects:** Full implementation with DogBrowserPage class
- **API Mocking:** cy.intercept() with fixtures
- **Coverage:** All exercises completed successfully

---

## Test Coverage Summary

| Test File               | Scenarios | Status   |
| ----------------------- | --------- | -------- |
| `homepage.cy.ts`        | 4         | Pass     |
| `fetch-dog.cy.ts`       | 5         | Pass     |
| `api-mocking.cy.ts`     | 4         | Pass     |
| `api-validation.cy.ts`  | 3         | Pass     |
| `custom-commands.cy.ts` | 3         | Pass     |
| `fixtures.cy.ts`        | 2         | Pass     |
| `page-objects.cy.ts`    | 3         | Pass     |
| `user-journey.cy.ts`    | 1         | Pass     |
| **TOTAL**               | **25+**   | **Pass** |

---

## Test Execution

### Interactive Mode

```bash
cd gui-testing
pnpm dev

# Terminal 2
pnpm exec cypress open
```

**Screenshot:** `/practical_8/screenshots/image.png`

### Headless Mode

```bash
cd gui-testing
pnpm exec cypress run
```

**Screenshot:** `/practical_8/screenshots/image1.png`

---

## Exercise Implementations

### Exercise 1: Homepage Display Testing

Tests page load, title display, placeholder messages, and breed selector population.

**Test Functions:**

- Page title validation
- Placeholder message display
- Breed selector population
- Button states and transitions

---

### Exercise 2: User Interaction Testing

Tests button clicks, image loading, breed filtering, and error handling.

**Test Functions:**

- Random dog image loading
- Loading state indicators
- Multiple sequential fetches
- Breed-specific filtering
- Error handling and recovery

---

### Exercise 3: API Mocking Implementation

Tests API request interception, response mocking, and validation.

**Implementation:**

```typescript
cy.intercept("GET", "/api/dogs", {
  fixture: "dog-responses.json",
}).as("getDog");
```

**Test Functions:**

- Mock successful API responses
- Mock breed list data
- Mock error responses
- Verify network calls

---

### Exercise 4: Response Validation

Tests API response structure, image URLs, and breed data integrity.

**Test Functions:**

- Response structure validation
- Image URL validation
- Breed data validation

---

### Exercise 5: Advanced Testing Patterns

Implements custom commands, page objects, and fixtures.

**Custom Commands:**

1. `cy.fetchDog()` - Fetch random dog and wait for image
2. `cy.selectBreedAndFetch(breed)` - Select breed and fetch dog
3. `cy.waitForDogImage()` - Wait for image to load

**Page Objects:**

DogBrowserPage class with centralized selectors and methods:

```typescript
class DogBrowserPage {
  pageTitle = '[data-testid="page-title"]';
  breedSelector = '[data-testid="breed-selector"]';
  fetchButton = '[data-testid="fetch-dog-button"]';
  dogImage = '[data-testid="dog-image"]';
  errorMessage = '[data-testid="error-message"]';

  visitPage() {
    /* ... */
  }
  clickFetchButton() {
    /* ... */
  }
  selectBreed(breed) {
    /* ... */
  }
}
```

**Fixtures:**

```json
{
  "status": "success",
  "message": "https://images.dog.ceo/breeds/retriever-golden/n02099601_1003.jpg"
}
```

---

## Complete User Journey

Test verifies full workflow:

1. User visits homepage
2. Sees welcome message and breed selector
3. Selects specific breed (corgi)
4. Fetches dog image
5. Switches to different breed (poodle)
6. Fetches another image
7. Selects "All Breeds" and fetches random dog

Result: Complete workflow executes without errors

---

## Technical Details

### Environment

- OS: Linux (Kali GNU/Linux Rolling)
- Node: 18.0+
- Cypress: 15.5.0+
- Next.js: 16.0.0
- TypeScript: 5.0+

### Configuration

```typescript
export default defineConfig({
  e2e: {
    baseUrl: "http://localhost:3000",
    viewportWidth: 1280,
    viewportHeight: 720,
  },
});
```

---

## Issues & Solutions

| Issue                  | Solution                                             | Result               |
| ---------------------- | ---------------------------------------------------- | -------------------- |
| Tests timing out       | Increased timeout to 10000ms, used cy.intercept()    | Tests run reliably   |
| Flaky tests            | Replaced real API with fixtures, explicit assertions | 100% pass rate       |
| Element not found      | Added data-testid attributes, proper wait strategies | All selectors stable |
| Inconsistent test data | Created fixtures, mocked all API calls               | Consistent results   |

---

## Conclusion

The practical successfully implemented comprehensive GUI testing with Cypress:

- 25+ test scenarios across 8 test files
- 100% pass rate
- 3 custom commands for reusable logic
- Full Page Objects pattern implementation
- API mocking with fixtures
- Complete user journey validation

---
