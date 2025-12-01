# Martyrs Management System

A JavaFX-based desktop application for managing martyrs data using advanced data structures including AVL trees, circular doubly linked lists, stacks, and queues.

## Prerequisites

- **Java 21** or higher
- **Maven 3.6+** (for dependency management)
- **JavaFX 21** (automatically managed by Maven)

## Project Structure

```
DataStructure_Project_3/
├── src/                    # Source code files
│   ├── Driver.java        # Main application entry point
│   ├── AVLTreeDate.java   # AVL tree implementation for dates
│   ├── AVLTreeName.java   # AVL tree implementation for names
│   ├── CircularDoublyLinkedList.java
│   ├── LinkedList.java
│   ├── Stack.java
│   ├── Queue.java
│   └── ...                # Other source files
├── bin/                   # Compiled classes (Eclipse)
├── target/                # Maven build output
├── pom.xml               # Maven configuration
├── btselem.csv           # Data file
├── btselem-copy.csv      # Backup data file
└── Martyrs.txt           # Output file
```

## Building and Running

### Using Maven (Recommended)

1. **Compile the project:**
   ```bash
   mvn clean compile
   ```

2. **Run the application:**
   ```bash
   mvn javafx:run
   ```

### Using Eclipse IDE

1. Import as Maven project: File → Import → Existing Maven Projects
2. Right-click on `Driver.java`
3. Run As → Java Application

### Using IntelliJ IDEA

1. Open the project folder
2. Right-click on `Driver.java`
3. Run 'Driver.main()'

## Features

- **Location Management**: Manage different locations where martyrs are recorded
- **Martyrs Data**: Add, update, delete, and search martyrs information
- **Statistics**: View comprehensive statistics about martyrs
- **Data Structures**: 
  - AVL Trees for efficient searching and sorting
  - Circular Doubly Linked Lists for location management
  - Stacks for tracking maximum martyrs
  - Queues for data processing

## Data File Format

The application reads CSV files with the following structure:
- Name
- Date of Death
- Age
- Location
- District
- Gender
- Marital Status

## Configuration

The project uses Maven for dependency management. JavaFX dependencies are automatically downloaded and configured.

### Maven Configuration (pom.xml)

- **JavaFX Version**: 21.0.1
- **Java Version**: 21
- **Build Plugin**: javafx-maven-plugin

## Troubleshooting

### JavaFX Not Found Error

If you encounter JavaFX-related errors:
1. Ensure Maven dependencies are updated: `mvn dependency:resolve`
2. Reload Maven project in your IDE
3. Use Maven to run: `mvn javafx:run`

### Missing Image Files

The application looks for:
- `palestine-logo.png` (icon)
- `background1.jpg` (background)

If these are missing, the app will use fallback options (text/default background).

## Notes

- The application was successfully configured to work with Maven and JavaFX 21
- All Eclipse configuration files have been updated for Maven integration
- Image loading includes error handling for missing resources
- Compatible with Java 21 and modern development environments

## License

Educational project for Data Structures course.
