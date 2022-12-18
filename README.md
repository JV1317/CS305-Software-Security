# CS305-Software-Security

### Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?
<p> Artemis Financial is a financial consulting company that handles sensitive information regarding their customers. They have hired Global Rain to analyze and address security vulnerabilities with their online application. It is imperative that secure communications be used when transmitting information across the network as well as storing that information in a secure way to ensure that information is not intercepted or accessed by others with malicious intent. Secure communication means that the company is using the necessary protocols and interfaces to send and receive data between the client and server.</p>

### What did you do very well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?
<p> I think I did a very good job of analyzing and identifying security vulnerabilities within the client’s software and recommending and implementing the appropriate fixes to address those vulnerabilities. Secure coding ensures that you are not exposing the application and therefor the company to vulnerabilities that can be leveraged to access the application or sensitive data within the system. By following the industries best practices and guidelines with respects to software security you are ensuring that your system and its data remain secure. </p>

### What part of the vulnerability assessment was challenging or helpful to you?
<p> The vulnerability assessment tool is an extremely beneficial tool as it will help to indicate vulnerabilities and dependencies within your application previously found by others and can help provide information on how to resolve them. I did not find the tool difficult to use but I do think it has some issues that need to be addressed. For example when attempting to suppress vulnerabilities I encountered several that were unable to be suppressed, even after adding them to the suppression file in the same manner as the others. </p>

### How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?
<p> We added layers of security to the application by first generating certificates for the application using the Java Keytool and by enabling the use of HTTPS. This allows for secure communication as well as providing authentication to our users so they can be sure they are using the authentic site an not an imposter. We then implemented a hashing function and ensured it was working correctly with the use of a check sum. The hash function will allow us to hash information and with the use of SHA-256 the possibility of collision is nearly impossible. 

Finally we insured that we introduced no new vulnerabilities into the system when we refactored our code. By using the most recent version of the OWASP maven dependency check we were able to confirm that after our code was refactored no new vulnerabilities were introduced. Ensuring that all dependencies and vulnerabilities are addressed will help provide security to the application. 
  
In the Future I plan to utilize dependancy check tools that are availabe like the OWASP dependency check tool we utilized in this class. I will then use the CVE database to investigate and find the best plan to mitigate any vulnerabilities that are found. 
 </p>

### How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?
<p>To ensure that the application was functional and secure I performed static and dynamic testing looking for any errors or new vulnerabilities that would have appeared after I refactored the code. To make sure there were no new vulnerabilities introduced I performed a static dependency check before I refactored the code. Once the code was refactored and the serverController class was added utilizing the check sum and hash functions, I ran another dependency check and compared the results from the two files.  </p>

### What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?
<p> The Maven dependency check tool paired with the national vulnerabilities database proved to be extemly useful tools for identifying and mitigating vulnerabilities within our program and I plan on utilizing both these tools in the future.  </p>

### Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?
<p> What I would like to show future employers from this assignment is the knowledge and skill required to use the tools available to develop an application with security in mind. Knowing how to find vulnerabilities and research to determine a method to mitigate those vulnerabilities is an especially useful skill that I believe would be relevant in the workplace. I think I would also like to highlight the knowledge of how certificates work and how to generate and apply them to an application as these are skills that will be very much relevant in the real world. </p>
