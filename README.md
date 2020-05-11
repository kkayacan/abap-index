

# abap-index
Hierarchical index of all topics for ABAP programming language

# ABAP - Dictionary
## 1. Classic objects in ABAP Dictionary
### 1.1. Data types
#### 1.1.1. Data elements
##### 1.1.1.1. Technical Attributes of Data Elements
###### 1.1.1.1.1. Elementary type
- Built-in data type
- Domain
###### 1.1.1.1.2. Reference type
`DATA | OBJECT`
##### 1.1.1.2. Semantic Attributes of Data Elements
- Short text
- Field label
- Documentation
- Supplement documentation
- Documentation status
- Search help
- SPA/GPA parameter
- Flag for input history
- Flag for bidirectional fonts
- Default component name
- Flag for change document
- Further semantic attributes in the domain
##### 1.1.1.3. Domains
###### 1.1.1.3.1. Technical Attributes of Domains
- Built-in data type in ABAP Dictionary
- Length
- A number of decimal places
###### 1.1.1.3.2. Semantic Attributes of Domains
- Short text
- Documentation
- Output attributes
	- Output length
	- Output style
	- Conversion routine
	- Sign
	- Lowercase letters
	- Time format
- Value range
- Value table
#### 1.1.2. Structures
##### 1.1.2.1. Technical attributes of structures
- Component name
- Component type
- Enhancement category
- Activation type
##### 1.1.2.2. Semantic attributes of structures 
- Short text of the structure
- Documentation
- Short text of components
- Output style of components
- Reference field
- Check table
- Search help
- Key field and flag for initial values
##### 1.1.2.3. Dictionary DDL for Structure Definitions
`DEFINE STRUCTURE`
#### 1.1.3. Table types
- Technical Attributes of Table Types
	- Row type
	- Table category
	- Table key
	- Initial row count
- Semantic Attributes of Table Types
	- Short text of the table type
	- Documentation
	- Short description of a secondary key
- Ranges Table Type
#### 1.1.4. Type Groups
`TYPE-POOL`
### 1.2. Database tables
- Technical attributes of database tables
	- Structure-Specific Technical Attributes of Database Tables
		- Table fields (columns)
		- Include structures
		- Enhancement category
	- Table-Specific Technical Attributes of Database Tables
		-   Table category
			- Transparent tables
			- Global temporary tables
		-   Data class
		-   Size category
		-   Logging
		-   Table buffering
			- Buffering Permission
			- Buffering Type
		-   Storage type
		-   Activation type
-	Semantic attributes of database tables
	-	Structure-Specific Semantic Attributes of Database Tables
		-   Short text
		-   Documentation
		-   Short text of table fields
		-   Output style of table fields
		-   Reference field
		-   Search help
	- Table-Specific Semantic Attributes of Database Tables
		-   Key fields
		-   Client dependency
		-   Foreign key dependencies
			- Check table
			- Foreign Key
				- Input check
				- Generic foreign key fields
				- Constant values
				- Inheritance
				- Cardinality
				- Type of the foreign key fields
		-   Flag for initial value
		-   Delivery class
		-   Secondary indexes
			- Primary Index
			- Secondary Indexes
			- Full Text Index
		-   Display and editing
- Global temporary tables
- Dictionary DDL for Defining Database Tables
`DEFINE TABLE`
- Updating (Converting) database tables
### 1.3. Views
- Classic Views 
	-   Database views
		- Basis Tables
		- View Fields
		- Join Conditions
		- Maintenance Status
		- Table Buffering
	-   Projection views
	-   Maintenance views
		- Primary Table and Secondary Tables
		- Time-Dependent Key
		- Maintenance Status
		- Maintenance Characteristics of View Fields
		- Delivery Class
	-   Help views
- External Views
### 1.4. Lock objects
`A lock object is used as a basis for SAP locks.`
### 1.5. Search helps
`A repository object that is used to create value lists.`
### 1.6. Tools for Classic ABAP Dictionary
- The ABAP Dictionary Tool in ABAP Workbench
- Tools in ADT
	- Form-Based Tools
	- Source-code-based tools
## 2. Objects in ABAP CDS
- Syntax
	- General Syntax Rules
	- Language Elements
- Annotations
	- Defining annotations
	- Specifying annotations
	- Evaluating annotations
	- SAP annotations
- Data Definitions
	- Views
	- Table Functions
	- Abstract CDS Entities
- Access Control
## 3. Dependency rules
`DEFINE DEPENDENCY RULE`
## 4. Built-in data types in ABAP Dictionary
-	Overview of All Built-In Dictionary Types
	-	General Types
		-	Numeric Types
			`INT1 | INT2 | INT4 | INT8 | DEC | DF16_DEC | DF16_RAW | DF34_DEC | DF34_RAW | FLTP`
		-	Character-Like Types
			`CHAR | LCHR | SSTRING | STRING`
		-	Byte-Like Types
			`RAW | LRAW | RAWSTRING`
	-	Special Types
		-	Date Types/Time Types
			`DATS | TIMS | ACCP`
		-	Character-Like Types with Special Semantics
			`NUMC | CLNT | LANG`
		-	Currency Fields and Quantity Fields
			`CURR | CUKY | QUAN | UNIT`
	-	Obsolete Types
		`DF16_SCL | DF34_SCL | PREC | VARC`
-	Attributes of the Built-In Dictionary Types
	-   General dictionary types
		-   Integers, packed numbers, binary floating point numbers
		-   Decimal floating point numbers
			- Handling in ABAP Dictionary
			- Handling in Dynpros - Output Length and Output Style
			- Handling in ABAP Programs
		-   Character-like types and byte-like types
			- Character Strings
			- Byte Chains
			- Notes on Strings
			- Use in ABAP SQL
			- Handling in Dynpros
	-   Special dictionary types
		- Date types and time types
		- Special character-like types
		- Currency fields
			- Handling in ABAP Dictionary
			- Handling in Dynpros
			- Handling in ABAP Programs
		- Quantity fields
			- Handling in ABAP Dictionary
			- Handling in Dynpros
			- Handling in ABAP Programs
	-   Obsolete dictionary types
-	Use of the Built-In Dictionary Types
## 5. Built-in database functions
### 5.1. SQL functions
#### 5.1.1. SQL functions for numeric values
`ABS | CEIL | DIV | DIVISION | FLOOR | MOD | ROUND`
#### 5.1.2. SQL functions for strings
`CONCAT | CONCAT_WITH_SPACE | INSTR | LEFT | LENGTH | LOWER | LPAD | LTRIM | REPLACE | RIGHT | RPAD | RTRIM | SUBSTRING | UPPER`
#### 5.1.3. SQL functions for null values
`COALESCE`
### 5.2. Special functions
#### 5.2.1. Conversion Functions
`FLTP_TO_DEC | BINTOHEX | HEXTOBIN | UNIT_CONVERSION | CURRENCY_CONVERSION | DECIMAL_SHIFT`
#### 5.2.2. Date Functions and Time Functions
`DATS_IS_VALID | DATS_DAYS_BETWEEN | DATS_ADD_DAYS | DATS_ADD_MONTHS | TIMS_IS_VALID | TSTMP_IS_VALID | TSTMP_CURRENT_UTCTIMESTAMP | TSTMP_SECONDS_BETWEEN | TSTMP_ADD_SECONDS | TSTMP_TO_DATS | TSTMP_TO_TIMS | TSTMP_TO_DST | DATS_TIMS_TO_TSTMP | ABAP_SYSTEM_TIMEZONE | ABAP_USER_TIMEZONE`
## 6. Activating ABAP Dictionary Types
- Runtime Objects
- Activating Dependent Objects
	- Activating Dependent ABAP Programs and Dynpros
	- Activating Dependent Dictionary Objects
`The system program RUTMSJOB can be used to deal with "partially active" objects.`
- Mass Activation
- Cyclical Dependencies

# ABAP − Reference
## 1. ABAP Syntax
-   ABAP statements
	- ABAP words
	- Operands
		- Names for operands
			- Structure Component Selector
			- Object Component Selector
			- Class Component Selector
			- Interface Component Selector
			- Dereferencing Operator
			- Chainings
		- Escape character for names
		- Specifying operands
			- Static Specification
			- Specifying Names Dynamically in Parentheses
			- Specifying Names Dynamically
		- Operand type
			- Operand Positions for Elementary Data Objects
			- Operand Positions for Structures
			- Operand Positions for Internal Tables
			- Operand Positions for Reference Variables
		- Data objects in operand positions
			- Read positions
			- Write positions
			- Subfield access (Substrings)
		- Functions and expressions in operand positions
			- Functions and Expressions for Operand Positions
				- Writing Positions
				- Reading Positions
			- Operand Positions for Functions and Expressions
				- Writer Positions
					- Declaration Positions
						- Positions for the inline declaration of variables
							- Left side of an assignment with the assignment operator =
							- Actual parameters for output parameters and return values of methods for standalone method calls
							- Target fields when catching an exception
							- Target fields in statements for string processing and byte string processing
							- Target fields in statements for time stamps
							- Target fields in statements for internal tables
							- Target fields of the ABAP SQL statement SELECT
							- Target fields of the statement DESCRIBE
							- Target fields of various GET statements
							- Work area in statement for dynpros
							- Target field for message output
							- Target fields in file interface statements
							- Target field for a serialization
							- All writing positions used when generating programs
						- Positions for the inline declaration of field symbols
							- Field symbol in the statement ASSIGN
							- Field symbols in statements for internal tables
					- Result Positions
						- Left side of an assignment with the assignment operator =
						- Operand dobj of the statement CLEAR
						- Memory area mem_area of the statement ASSIGN mem_area TO
						- Structure struc of the statement ASSIGN COMPONENT comp OF STRUCTURE struc
						- Actual parameter in method calls for output parameters, input/output parameters, and return values
						- The right side in the declaration of a local field symbol in a LET expression
				- Reader Positions
					- General Expression Positions
						- Right side of an assignment with the assignment operator =
						- Operands of arithmetic expressions and of bit expressions
						- Embedded expressions in string templates
						- Operands of comparison expressions in logical expressions
						- Operand of the statement CASE
						- Actual parameters for input parameters of methods in meth( ... ), RAISE EVENT, CREATE OBJECT, and RAISE EXCEPTION or THROW in a conditional expression
						- Actual parameters for input parameters of function modules in the case of CALL FUNCTION
						- Arguments of built-in numeric functions if they are themselves executed in an arithmetic expression
						- Reference variable oref of statement RAISE EXCEPTION oref.
						- The operands behind the addition WITH TABLE KEY of the statements READ TABLE itab and DELETE TABLE itab
						- The operands behind the addition WITH KEY of the statement READ TABLE itab
						- Work area wa
						- Expression exp for dynamic sorts
						- Source fields of the statements WRITE and WRITE TO
					- Numeric Expression Positions
						- Arguments of functions
						- Counters and positions
						- Positions specified in the statements FIND and REPLACE
						- The row number idx specified with respect to a table index when accessing an internal table		
					- Character-Like Expression Positions
					- Time-Stamp-Like Expression Positions
					- Functional Operand Positions
	- Operators
		- Operators that perform special operations in operand positions
			- Declaration Operators `DATA | FIELD-SYMBOL`
			- Constructor Operators `NEW | VALUE | CONV | CORRESPONDING | CAST | REF | EXACT | REDUCE | FILTER | COND | SWITCH`
		- Operators that join multiple operands in a single expression
			- Assignment Operators `= | ?= | += | -= | *= | /= | &&=`
			- Arithmetic Operators `+ | - | * | / | DIV | MOD | **`
			- Bit Operators `BIT-AND | BIT-OR | BIT-XOR | BIT-NOT`
			- String Operators `&&`
			- Relational Operators `= | <> | < | > | <= | >= | BETWEEN`
			- Boolean Operators `AND | OR | EQUIV | NOT`
		- Operator that joins two operands in compilations
			- Literal Operator `&`
	- Expressions
		- Writer positions
			- Declaration expressions
			- Certain constructor expressions
			- Certain table expressions
		- Reader positions
			- Logical expressions
			- Constructor expressions
			- Table expressions and mesh path expressions
			- Arithmetic expressions
			- String expressions
			- Bit expressions
-   Naming conventions
-   Chained statements 
-   Comments  
-   Program directives  
-   Syntax conventions
## 2. Program Layout
## 3. Predefined Types, Data Objects, and Functions
## 4. Declarations
## 5. Creating Objects and Values
## 6. Calling and Exiting Program Units
## 7. Controlling the Program Flow
## 8. Processing Internal Data
## 9. Processing External Data
## 10. Text Repositories
## 11. Language Environment
## 12. Program Processing
## 13. Data Interfaces and Communication Interfaces
## 14. SAP GUI User Dialogs
## 15. Enhancements
## 16. Obsolete Language Elements