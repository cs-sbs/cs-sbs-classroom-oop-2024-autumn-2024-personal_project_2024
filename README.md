### 课程项目描述：图书管理系统

**项目目标**：
本项目要求学生基于面向对象的设计思想，开发一个控制台的图书管理系统。
系统中将包含多种不同类型的图书，每种图书根据类别有不同的属性和方法。
学生需要应用类和对象、继承、多态和封装等核心面向对象编程概念，
并进一步学习多线程、数据库操作和文件流的应用，实现一个可扩展、模块化的图书管理系统。
本项目使用控制台交互，强化程序的逻辑设计和面向对象编程概念的应用。


---

#### 1. **功能要求**
   - **用户注册和登录**：
     - 系统需要包含两个用户角色：普通用户和管理员。普通用户可以查看和搜索图书信息，管理员可以增删图书。
   - **书籍管理**：
     - 图书添加：能够添加新的图书，包括通用信息（如书名、作者、出版日期等）和特定类别信息。
     - 图书查询：支持查询图书信息，允许用户根据书名、ISBN等关键字查询，并显示所有相关信息。
     - 图书删除：支持从系统中删除图书。
     - 图书分类筛选：按类别展示图书，例如显示所有计算机类、医学类、文学类、法学类等书籍。
   - **面向对象特性要求**：
     - 类和对象：创建一个基类，以便支持不同类型图书的扩展。
     - 继承：设计若干子类，基于图书的不同分类进行继承和扩展。子类需在基类的基础上新增特定属性和方法，以体现不同类型图书的特性。
     - 封装：所有类的属性需使用封装，确保数据的私密性和安全性。提供适当的访问方法，以控制对类内数据的访问和修改。
     - 多态：在父类或接口中定义展示信息的方法，要求子类进行具体实现。系统应能通过多态性，调用不同子类的展示方法，输出类型特定的信息。
   - **文件存储与读取**：使用文件流将图书信息存储为文件，保证系统重新启动时数据的持久化。
   - **多线程支持**：系统需要实现一个数据定期备份功能，备份操作应在后台独立线程中进行，不影响用户的正常操作。
   - **数据库支持**：书籍数据应存储在数据库中，学生可以选择MySQL或SQLite数据库。
---

#### 2. 交互方式
- **命令行菜单**：
   创建一个简洁的控制台菜单，比如：

   ```
   Welcome to the Book Management System
   1. Register
   2. Login
   3. View Books
   4. Search Books
   5. Add a Book（Admin Only）
   6. Delete a Book（Admin Only）
   7. Logout
   8. Exit
   Please enter your choice: _
   ```
   提示用户输入对应数字选择操作，并通过循环保持菜单的持续交互性。

---

#### 3. **高级功能要求**
   - **多线程**：
     - 实现一个后台线程，定期将数据库中的书籍数据备份到文件中。
   - **数据库操作**：
     - 使用JDBC进行数据库连接、数据增删查改。
   - **文件流**：
     - 使用文件流将备份文件进行读取和写入，支持备份文件的恢复功能。

---

#### 4. **评分标准**
   - **功能完整性（50%）**：
     - 基本功能（30%）：用户注册、登录，图书的增删查改功能，控制台界面。
     - 高级功能（20%）：多线程数据备份、文件存储和读取、数据库操作。
   - **面向对象设计（30%）**：
     - 类的设计合理性、继承关系、封装性、多态性的正确使用。
   - **代码质量（20%）**：
     - 代码结构清晰，命名规范，注释完整，代码风格符合规范。

#### 5. **提交要求**
   - **项目代码**：包含所有源代码文件，确保可以编译和运行。
   - **数据库脚本**：提供数据库表的创建脚本及测试数据。
   - **项目说明文档**：简单说明系统设计、类的结构图、运行方式及功能描述。
   - **截止日期： 2025-01-05 23:59**

通过本项目，学生可以全面应用Java的面向对象编程和多线程、数据库操作等高级技术，为今后的Java开发打下坚实基础。