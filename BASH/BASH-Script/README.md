# What You Will Learn

## At the Core of the Lesson

In this lesson, you will learn how to:

- Describe common tasks accomplished through shell scripts
- Use basic commands frequently included in shell scripts
- Understand basic logical control statements often included in shell scripts
- Execute a shell script
# What Are Scripts?

Scripts are text files containing commands and related data. When the text file is processed, the commands are executed. Here are key points about scripts:

- **Processing:** Scripts are processed to run the specified commands.

- **Scheduling:** Scripts can be set as scheduled tasks using tools like cron.

- **Automation Benefits:** Automation allows scripts to run more quickly than manual execution. It also ensures consistency by removing the potential for manual errors.

## Common Script Tasks

Scripts are versatile and commonly used for various tasks, including:

- **Creating Backup Jobs**
- **Archiving Log Files**
- **Configuring Systems and Services**
- **Simplifying Repetitive Tasks**
- **Automating Tasks**
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/181a830f-e9aa-4191-82e2-e7ed6b14bc4f)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/70671191-2ca3-428a-b116-72232a365154)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/20c9ed15-82b6-4251-8495-5a761282d3ee)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/8d49f052-5209-4e88-b64c-cc10d858e2a9)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/3abf7b6d-f669-4553-9a88-7fa66964d997)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/3604297c-6956-47e9-87e6-daa3ab4c0124)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/6634b30c-f4fa-4d9e-9ffe-df44d27246a1)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/afaa928b-b5b0-4d94-a094-8993be7f1704)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/223a0a4c-662f-44c5-aa12-cd19c25a9780)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/aca7ae98-08b8-44b8-a52e-c30c0b935651)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/bb703eef-c0c0-40ec-beca-72f3009d0b50)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/74edaabe-8bf8-4a4e-9fdb-29ba3941a7a0)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/03c7aa1d-c1ab-418a-b58a-83f607d7dec3)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/13001934-9ec8-41c5-8de5-99b51677e168)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/4def3db5-5fd0-4c1c-b606-f65d12f43678)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/b3abaf5f-eb25-4f57-a8ae-5a7fa314d91b)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/851fc830-3c05-466d-89f8-cc1f46eec7a4)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/bd574ec1-781e-4afd-8f09-46523fe18209)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/9d90ae08-0fd0-4b95-b7b2-d8e121230362)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/7508cb78-7b02-4542-bb4f-c20f6a44c3b1)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/a0b6f40f-2f35-439d-a92f-ef92a50ee444)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/b9c5dce1-ffaf-4453-ac39-043e69c68075)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/e3c065ee-f845-480b-99df-518d60bac742)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/6040aeea-e4b1-4946-8c70-a4f991963611)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/b3e57581-7093-43cb-853e-cee6e074e89e)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/5150a5a9-23ac-46b4-a75b-2b6caaa629ee)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/ee558844-be65-4415-afb9-0cd101ed36f9)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/efc333f8-94dd-4ef4-b50e-b0dc6e10908b)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/affe3531-4686-459e-a661-a676a3e2dfdb)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/8d31ba8d-d5f2-4105-be46-4f242f721c5d)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/644f0c98-0e5e-404a-b798-c38bef4f8dd2)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/4c12e44b-c968-4a1c-bf49-e75ea842eeb1)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/b75aa73a-4516-4080-8b95-7442941e5580)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/12d213fc-96bd-477f-9479-80b055f31bf5)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/ee01b70a-acfd-434e-b5cc-0103820d276a)
![image](https://github.com/gauravhalnawar1011/AWS/assets/140076717/63db56da-26df-4be0-bb8b-b8aec1f636d6)
![Uploading image.png…]()
