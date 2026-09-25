## 📋 Project Assessment: Lab #11 - File IO (Plant Archive)

### 1. Development & Workflow
- [ ] **Commit Messages:** Descriptive, incremental commits tracking CSV parsing, stream initialization, and list output.

### 2. Functional Requirements

#### Step 1: Model Upgrade & CSV Parsing (`Plant.java`)
- [ ] **CSV Constructor:** Created single-parameter constructor `Plant(String csvLine)` accepting a CSV line.
- [ ] **String Splitting:** Correctly used `String.split(",")` to tokenize CSV fields.
- [ ] **Data Assignment:** Instance variables populated with parsed and appropriately converted tokens (e.g., temperature ranges, uses, names).
- [ ] **Error Checking & Validation:**
    - [ ] Validated input string is not `null` or empty prior to splitting.
    - [ ] Verified split array length matches expected column count.
    - [ ] Handled potential data conversion/parsing errors gracefully.

#### Step 2: File Input Pipeline (`Main.java`)
- [ ] **Imports:** Imported necessary File I/O classes.
- [ ] **Stream Declaration & Initialization:**
    - [ ] Declared `FileInputStream` and `Scanner` variables.
    - [ ] Initialized streams pointing to `"Forage.csv"`.
- [ ] **Exception Handling:** Handled `FileNotFoundException` or wrapped I/O operations in a try-catch block.
- [ ] **Reading Loop:** Implemented loop to read through all records.
- [ ] **Resource Management:** Closed both input streams after processing.

#### Step 3: Object Construction & Display Output (`Main.java`)
- [ ] **List Storage:** Instantiated `ArrayList<Plant>` to store generated `Plant` objects.
- [ ] **Loop Population:** Built a new `Plant` object per line iteration and appended it to the `ArrayList`.
- [ ] **Console Display:** Printed `ArrayList` elements to the console with proper formatting/labels matching example output.

### 3. Code Quality & Standards
- [ ] **Exception Safety:** Proper handling of potential File I/O exceptions without unhandled crashes.
- [ ] **Encapsulation:** Retained `private` visibility for `Plant` instance variables.
- [ ] **Naming Conventions:** Standard `camelCase` for variables/methods and `PascalCase` for classes.
- [ ] **Formatting:** Clean structure and consistent indentation throughout I/O logic.
