- # Lab1：Kotlin 基础语法练习

  ## 实验背景

  本次实验涵盖 Kotlin 编程的基础语法，包括输出语句、变量、字符串操作、基本数学运算以及函数定义与调用。
   建议使用 [Kotlin Playground](https://play.kotlinlang.org/) 在线编写并运行代码，完成后将代码粘贴到对应代码块中提交。

  ------

  ## 提交要求

  ```
  学号姓名/
  └── Lab1/
      └── kotlin_basics.md    # 将答案填入本文件各题代码块后提交 
      												# 你需要把这份文件复制一份到你的文件夹
  ```
  
  截止时间：**2026-3-20**，届时关于 Lab1 的 PR 请求将不会被合并。
  
  ------
  
  ## 题目 2：输出消息
  
  使用 Kotlin Playground 编写一个程序，输出以下三行消息：
  
  ```
  I'm
  learning
  Kotlin!
  ```
  
  **你的答案：**
  
  ```kotlin
  // 请将完整代码粘贴至此
  ```
  
  ------
  
  ## 题目 3：修正编译错误
  
  以下每段代码都存在错误，请将它们复制到 Kotlin Playground，找出并修正错误，使程序能正常运行输出预期结果。
  
  **练习 3.1**
  
  ```kotlin
  fun main() {
      println("Tomorrow is rainy")
  ```
  
  预期输出：`Tomorrow is rainy`
  
  **你的答案：**
  
  ```kotlin
  // 请将修正后的完整代码粘贴至此
  ```
  
  ------
  
  **练习 3.2**
  
  ```kotlin
  fun main() {
      printLine("There is a chance of snow")
  }
  ```
  
  预期输出：`There is a chance of snow`
  
  **你的答案：**
  
  ```kotlin
  // 请将修正后的完整代码粘贴至此
  ```
  
  ------
  
  **练习 3.3**
  
  ```kotlin
  fun main() {
      println("Cloudy") println("Partly Cloudy") println("Windy")
  }
  ```
  
  预期输出：
  
  ```
  Cloudy
  Partly Cloudy
  Windy
  ```
  
  **你的答案：**
  
  ```kotlin
  // 请将修正后的完整代码粘贴至此
  ```
  
  ------
  
  **练习 3.4**
  
  ```kotlin
  fun main() (
      println("How's the weather today?")
  )
  ```
  
  预期输出：`How's the weather today?`
  
  **你的答案：**
  
  ```kotlin
  // 请将修正后的完整代码粘贴至此
  ```
  
  ------
  
  ## 题目 4：字符串模板
  
  请补全 `main()` 函数，使用 `$` 字符串模板将变量嵌入字符串中输出一条通知消息。
  
  初始代码：
  
  ```kotlin
  fun main() {
      val numberOfMessages = 5
      // 请使用字符串模板输出以下消息
  }
  ```
  
  预期输出：
  
  ```
  You have 5 unread messages.
  ```
  
  **你的答案：**
  
  ```kotlin
  // 请将完整代码粘贴至此
  ```
  
  ------
  
  ## 题目 5：字符串串联
  
  请编写程序，声明变量 `val nextDelivery = "Tuesday"`，通过字符串串联（`+` 运算符）输出以下消息。
  
  预期输出：
  
  ```
  Your package will arrive on Tuesday.
  ```
  
  **你的答案：**
  
  ```kotlin
  // 请将完整代码粘贴至此
  ```
  
  ------
  
  ## 题目 6：消息格式
  
  请编写程序，根据以下变量，使用字符串模板输出一条格式化的天气消息。
  
  变量：
  
  ```kotlin
  val city = "Austin"
  val lowTemp = 65
  val highTemp = 90
  val rainPercentage = 30
  ```
  
  预期输出：
  
  ```
  City: Austin
  Low: 65, High: 90
  Chance of rain: 30%
  ```
  
  **你的答案：**
  
  ```kotlin
  // 请将完整代码粘贴至此
  ```
  
  ------
  
  ## 题目 7：实现基本数学运算
  
  请声明 `val operandOne = 60` 和 `val operandTwo = 4`，输出以下所有运算结果。
  
  预期输出：
  
  ```
  60 + 4 = 64
  60 - 4 = 56
  60 / 4 = 15
  60 * 4 = 240
  60 % 4 = 0
  ```
  
  **你的答案：**
  
  ```kotlin
  // 请将完整代码粘贴至此
  ```
  
  ------
  
  ## 题目 8：默认参数
  
  请补全 `birthdayGreeting()` 函数，为 `name` 参数设置默认值 `"Rover"`，使得调用时不传 `name` 也能正常运行。
  
  初始代码：
  
  ```kotlin
  fun main() {
      println(birthdayGreeting(age = 5))
      println(birthdayGreeting("Rex", 2))
  }
  
  fun birthdayGreeting(name: String, age: Int): String {
      // 请在此填写代码，为 name 添加默认值并返回格式化祝语
  }
  ```
  
  预期输出：
  
  ```
  Happy Birthday, Rover! You are now 5 years old!
  Happy Birthday, Rex! You are now 2 years old!
  ```
  
  **你的答案：**
  
  ```kotlin
  // 请将完整代码粘贴至此
  ```
  
  ------
  
  ## 题目 9：计步器
  
  计步器是一种可计算行走步数的设备，函数会根据步数计算消耗的卡路里。请根据 Kotlin 命名最佳实践（camelCase），重命名以下程序中所有命名不规范的函数、参数和变量，程序逻辑不变。
  
  原始代码（命名不规范）：
  
  ```kotlin
  fun main() {
      val Steps = 4000
      val caloriesBurned = PEDOMETERstepsTOcalories(Steps)
      println("Walking $Steps steps burns $caloriesBurned calories")
  }
  
  fun PEDOMETERstepsTOcalories(NumberOFStepS: Int): Double {
      val CaloriesBURNEDforEachStep = 0.04
      val TotalCALORIESburned = NumberOFStepS * CaloriesBURNEDforEachStep
      return TotalCALORIESburned
  }
  ```
  
  **你的答案：**
  
  ```kotlin
  // 请将重命名后的完整代码粘贴至此
  ```
  
  ------
  
  ## 题目 10：比较两个数字
  
  请补全 `main()` 函数，使用 `if/else` 表达式比较两个数字并输出较大的那个。若两数相等，则输出 `First and second are equal.`
  
  初始代码：
  
  ```kotlin
  fun main() {
      val first = 35
      val second = 27
      // 请在此填写代码
  }
  ```
  
  预期输出：
  
  ```
  35
  ```
  
  **你的答案：**
  
  ```kotlin
  // 请将完整代码粘贴至此
  ```
  
  ------
  
  ## 题目 11：将重复代码移至一个函数中
  
  以下程序重复输出多个城市的天气信息，存在大量重复代码。请创建一个函数消除重复，并用该函数替代 `main()` 中所有重复的 `println()`。
  
  原始代码：
  
  ```kotlin
  fun main() {
      println("City: Ankara")
      println("Low temperature: 27, High temperature: 31")
      println("Chance of rain: 82%")
      println()
  
      println("City: Tokyo")
      println("Low temperature: 32, High temperature: 36")
      println("Chance of rain: 10%")
      println()
  
      println("City: Cape Town")
      println("Low temperature: 59, High temperature: 64")
      println("Chance of rain: 2%")
      println()
  
      println("City: Guatemala City")
      println("Low temperature: 50, High temperature: 55")
      println("Chance of rain: 7%")
      println()
  }
  ```
  
  **你的答案：**
  
  ```kotlin
  // 请将完整代码粘贴至此
  ```
  
  ------
  
  ## 参考资料
  
  - [Kotlin Playground](https://play.kotlinlang.org/)
