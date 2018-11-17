# Penetration Test Guide based on the OWASP + Extra
This guid is for the penetration testers seeking for the appropriate test cases required during a penetration test project. I rearranged the [OWASP Testing Guide v4](https://www.owasp.org/index.php/OWASP_Testing_Guide_v4_Table_of_Contents) from my point of view including `9 Test Classes` and each class has several `Test Cases` to conduct against the target. Each `Test Case` covers several OWASP tests which also is useful for the report document. I've also added `10 extra Tests Cases` marked by the `EXTRA-TEST`. I hope it will be useful in both penetration test projects and bug-bounty.

### TODO: 
1. Add resources for each test

## Information Gathering
*   *    **Fingerprint Technologies**
    *    Fingerprint Web Server ([OTG-INFO-002](https://www.owasp.org/index.php/Fingerprint_Web_Server_(OTG-INFO-002)))
    *    Enumerate Applications on Webserver ([OTG-INFO-004](https://www.owasp.org/index.php/Enumerate_Applications_on_Webserver_(OTG-INFO-004)))
    *    Fingerprint Web Application Framework ([OTG-INFO-008](https://www.owasp.org/index.php/Fingerprint_Web_Application_Framework_(OTG-INFO-008)))
    *    Fingerprint Web Application ([OTG-INFO-009](https://www.owasp.org/index.php/Fingerprint_Web_Application_(OTG-INFO-009)))
*   *    Information Leakage
    *    Conduct Search Engine Discovery and Reconnaissance for Information Leakage ([OTG-INFO-001](https://www.owasp.org/index.php/Conduct_search_engine_discovery/reconnaissance_for_information_leakage_(OTG-INFO-001)))
    *    Review Webserver Metafiles for Information Leakage ([OTG-INFO-003](https://www.owasp.org/index.php/Review_Webserver_Metafiles_for_Information_Leakage_(OTG-INFO-003)))
    *    Review Webpage Comments and Metadata for Information Leakage ([OTG-INFO-005](https://www.owasp.org/index.php/Review_webpage_comments_and_metadata_for_information_leakage_(OTG-INFO-005)))
    *    Analysis of Error Codes ([OTG-ERR-001](https://www.owasp.org/index.php/Testing_for_Error_Code_(OTG-ERR-001)))
    *    Analysis of Stack Traces ([OTG-ERR-002](https://www.owasp.org/index.php/Testing_for_Stack_Traces_(OTG-ERR-002)))
*   *    Directory Indexing
    *    Search for Directory Indexing (EXTRA-TEST-001)
## Configuration and Deployment Management

*   *    Enumerate Infrastructure and Application Admin Interfaces
    *    Enumerate Infrastructure and Application Admin Interfaces ([OTG-CONFIG-005](https://www.owasp.org/index.php/Enumerate_Infrastructure_and_Application_Admin_Interfaces_(OTG-CONFIG-005)))
    *    Test Network/Infrastructure Configuration ([OTG-CONFIG-001](https://www.owasp.org/index.php/Test_Network/Infrastructure_Configuration_(OTG-CONFIG-001)))
*   *    Hidden Resources Discovery
    *    Review Old, Backup and Unreferenced Files for Sensitive Information ([OTG-CONFIG-004](https://www.owasp.org/index.php/Review_Old,_Backup_and_Unreferenced_Files_for_Sensitive_Information_(OTG-CONFIG-004)))
*   *    HTTP Security Headers
    *    Testing for Lack of HTTP Security Headers (EXTRA-TEST-002)
## Identity Management and Authentication
*   *    Secure Authentication Class
    *    Test User Registration Process ([OTG-IDENT-002](https://www.owasp.org/index.php/Test_User_Registration_Process_(OTG-IDENT-002)))
    *    Testing for Weak Lock Out Mechanism ([OTG-AUTHN-003](https://www.owasp.org/index.php/Testing_for_Weak_lock_out_mechanism_(OTG-AUTHN-003)))
    *    Testing for Bypassing Authentication Schema ([OTG-AUTHN-004](https://www.owasp.org/index.php/Testing_for_Bypassing_Authentication_Schema_(OTG-AUTHN-004)))
    *    Test Remember Password Functionality ([OTG-AUTHN-005](https://www.owasp.org/index.php/Testing_for_Vulnerable_Remember_Password_(OTG-AUTHN-005)))
    *    Testing for Browser Cache Weakness ([OTG-AUTHN-006](https://www.owasp.org/index.php/Testing_for_Browser_cache_weakness_(OTG-AUTHN-006)))
    *    Testing for Weak Security Question/Answer ([OTG-AUTHN-008](https://www.owasp.org/index.php/Testing_for_Weak_security_question/answer_(OTG-AUTHN-008)))
    *    Testing for Weak Password Change or Reset Functionalities ([OTG-AUTHN-009](https://www.owasp.org/index.php/Testing_for_weak_password_change_or_reset_functionalities_(OTG-AUTHN-009)))
    *    Testing for Weaker Authentication in Alternative Channel ([OTG-AUTHN-010](https://www.owasp.org/index.php/Testing_for_Weaker_authentication_in_alternative_channel_(OTG-AUTHN-010)))
    *    Testing for Weak or Unenforced Username Policy ([OTG-IDENT-005](https://www.owasp.org/index.php/Testing_for_Weak_or_unenforced_username_policy_(OTG-IDENT-005)))
    *    Testing for Default Credentials ([OTG-AUTHN-002](https://www.owasp.org/index.php/Testing_for_default_credentials_(OTG-AUTHN-002)))
*   *    Username Enumeration
    *    Testing for Account Enumeration and Guessable User Account ([OTG-IDENT-004](https://www.owasp.org/index.php/Testing_for_Account_Enumeration_and_Guessable_User_Account_(OTG-IDENT-004)))
*   *    Testing for Recovering Sensitive Information
    *    Testing for Recovering Sensitive Information from Database (EXTRA-TEST-003)
*   *    Testing against Brute Force attack
    *    Testing against Brute Force attack (EXTRA-TEST-004)
*   *    Password policy
    *    Testing for Weak password policy ([OTG-AUTHN-007](https://www.owasp.org/index.php/Testing_for_Weak_password_policy_(OTG-AUTHN-007)))
*   *    Testing for SSL over User Authentication
    *    Testing for Credentials Transported over an Encrypted Channel ([OTG-AUTHN-001](https://www.owasp.org/index.php/Testing_for_Credentials_Transported_over_an_Encrypted_Channel_(OTG-AUTHN-001)))
## Authorization and Boundary Test
*   *    User Access Control
    *    Test Role Definitions ([OTG-IDENT-001](https://www.owasp.org/index.php/Test_Role_Definitions_(OTG-IDENT-001)))
    *    Test Account Provisioning Process ([OTG-IDENT-003](https://www.owasp.org/index.php/Test_Account_Provisioning_Process_(OTG-IDENT-003)))
    *    Testing for Bypassing Authorization Schema ([OTG-AUTHZ-002](https://www.owasp.org/index.php/Testing_for_Bypassing_Authorization_Schema_(OTG-AUTHZ-002)))
    *    Testing for Privilege Escalation ([OTG-AUTHZ-003](https://www.owasp.org/index.php/Testing_for_Privilege_escalation_(OTG-AUTHZ-003)))
    *    Testing for HTTP Verb Tampering ([OTG-INPVAL-003](https://www.owasp.org/index.php/Testing_for_HTTP_Verb_Tampering_(OTG-INPVAL-003)))
*   *    File Inclusions
    *    Testing Directory Traversal/File Include ([OTG-AUTHZ-001](https://www.owasp.org/index.php/Testing_Directory_traversal/file_include_(OTG-AUTHZ-001))
*   *    Execution after Redirect
    *    Execution after Redirect (EXTRA-TEST-005)
*   *    Cross Site Request Forgery
    *    Testing for Cross Site Request Forgery (CSRF) ([OTG-SESS-005](https://www.owasp.org/index.php/Testing_for_CSRF_(OTG-SESS-005)))
*   *    Secured File Upload
    *    Arbitrary File Upload (EXTRA-TEST-006)
    *    Test Upload of Unexpected File Types ([OTG-BUSLOGIC-008](https://www.owasp.org/index.php/Test_Upload_of_Unexpected_File_Types_(OTG-BUSLOGIC-008)))
    *    Test Upload of Malicious Files ([OTG-BUSLOGIC-009](https://www.owasp.org/index.php/Test_Upload_of_Malicious_Files_(OTG-BUSLOGIC-009)))
*   *    Insecure Direct Object References
    *    Testing for Insecure Direct Object References ([OTG-AUTHZ-004](https://www.owasp.org/index.php/Testing_for_Insecure_Direct_Object_References_(OTG-AUTHZ-004))) - [References](https://github.com/Voorivex/pentest-guide/tree/master/Testing-for-Insecure-Direct-Object-References)
*   *    Secured Captcha implementation
    *    Test for Secured Captcha Workflow (EXTRA-TEST-007)
    
## Cookie and Session Management
*   *    Testing for Cookies attributes
    *    Testing for Cookies attributes ([OTG-SESS-002](https://www.owasp.org/index.php/Testing_for_cookies_attributes_(OTG-SESS-002)))
*   *    Secure Session Management
    *    Testing for Bypassing Session Management Schema ([OTG-SESS-001](https://www.owasp.org/index.php/Testing_for_Session_Management_Schema_(OTG-SESS-001)))
    *    Testing for Session Fixation ([OTG-SESS-003](https://www.owasp.org/index.php/Testing_for_Session_Fixation_(OTG-SESS-003)))
    *    Testing for Exposed Session Variables ([OTG-SESS-004](https://www.owasp.org/index.php/Testing_for_Exposed_Session_Variables_(OTG-SESS-004)))
    *    Testing for Logout functionality ([OTG-SESS-006](https://www.owasp.org/index.php/Testing_for_logout_functionality_(OTG-SESS-006)))
    *    Test Session Timeout ([OTG-SESS-007](https://www.owasp.org/index.php/Test_Session_Timeout_(OTG-SESS-007)))
    *    Testing for Session puzzling ([OTG-SESS-008](https://www.owasp.org/index.php/Testing_for_Session_puzzling_(OTG-SESS-008)))
## Accessibility
*   *    Denial of Service
    *    Test for Denial of Service (EXTRA-TEST-008)
    
## Input/Output Validation
*   *    Cross Site Scripting
    *    Testing for Reflected Cross Site Scripting ([OTG-INPVAL-001](https://www.owasp.org/index.php/Testing_for_Reflected_Cross_site_scripting_(OTG-INPVAL-001)))
    *    Testing for Stored Cross Site Scripting ([OTG-INPVAL-002](https://www.owasp.org/index.php/Testing_for_Stored_Cross_site_scripting_(OTG-INPVAL-002)))
    *    Testing for DOM based Cross Site Scripting ([OTG-CLIENT-001](https://www.owasp.org/index.php/Testing_for_DOM-based_Cross_site_scripting_(OTG-CLIENT-001)))
    *    Testing for JavaScript Execution ([OTG-CLIENT-002](https://www.owasp.org/index.php/Testing_for_JavaScript_Execution_(OTG-CLIENT-002)))
    *    Testing for HTML Injection ([OTG-CLIENT-003](https://www.owasp.org/index.php/Testing_for_HTML_Injection_(OTG-CLIENT-003)))
    *    Testing for CSS Injection ([OTG-CLIENT-005](https://www.owasp.org/index.php/Testing_for_CSS_Injection_(OTG-CLIENT-005)))
    *    Testing for Client Side Resource Manipulation ([OTG-CLIENT-006](https://www.owasp.org/index.php/Testing_for_Client_Side_Resource_Manipulation_(OTG-CLIENT-006)))
    *    Testing for Clickjacking ([OTG-CLIENT-009](https://www.owasp.org/index.php/Testing_for_Clickjacking_(OTG-CLIENT-009)))
*   *    SQL Injection
    *    Testing for SQL Injection ([OTG-INPVAL-005](https://www.owasp.org/index.php/Testing_for_SQL_Injection_(OTG-INPVAL-005)))
    *    Testing for Incubated Vulnerabilities ([OTG-INPVAL-015](https://www.owasp.org/index.php/Testing_for_Incubated_Vulnerability_(OTG-INPVAL-015)))
*   *    Server Side Code Injection
    *    Testing for LDAP Injection ([OTG-INPVAL-006](https://www.owasp.org/index.php/Testing_for_LDAP_Injection_(OTG-INPVAL-006)))
    *    Testing for ORM Injection ([OTG-INPVAL-007](https://www.owasp.org/index.php/Testing_for_ORM_Injection_(OTG-INPVAL-007)))
    *    Testing for XML Injection ([OTG-INPVAL-008](https://www.owasp.org/index.php/Testing_for_XML_Injection_(OTG-INPVAL-008)))
    *    Testing for SSI Injection ([OTG-INPVAL-009](https://www.owasp.org/index.php/Testing_for_SSI_Injection_(OTG-INPVAL-009)))
    *    Testing for XPath Injection ([OTG-INPVAL-010](https://www.owasp.org/index.php/Testing_for_XPath_Injection_(OTG-INPVAL-010)))
    *    IMAP/SMTP Injection ([OTG-INPVAL-011](https://www.owasp.org/index.php/Testing_for_IMAP/SMTP_Injection_(OTG-INPVAL-011)))
    *    Testing for Code Injection ([OTG-INPVAL-012](https://www.owasp.org/index.php/Testing_for_Code_Injection_(OTG-INPVAL-012)))
*   *    Remote Command Execution
    *    Testing for Command Injection ([OTG-INPVAL-013](https://www.owasp.org/index.php/Testing_for_Command_Injection_(OTG-INPVAL-013)))
*   *    Buffer Overflow
    *    Testing for Buffer Overflow ([OTG-INPVAL-014](https://www.owasp.org/index.php/Testing_for_Buffer_Overflow_(OTG-INPVAL-014)))
*   *    XML External Entity (XXE)
    *    Testing for XML External Entity (XXE) (EXTRA-TEST-009)
*   *    Server Side Request Forgery (SSRF)
    *    Testing for Server Side Request Forgery (SSRF) (EXTRA-TEST-010)
*   *    Open Redirect
    *    Testing for Client Side URL Redirect ([OTG-CLIENT-004](https://www.owasp.org/index.php/Testing_for_Client_Side_URL_Redirect_(OTG-CLIENT-004)))
    
## Testing for weak Cryptography
*   *    Testing for Weak SSL/TLS Ciphers, Insufficient Transport Layer Protection
    *    Testing for Weak SSL/TLS Ciphers, Insufficient Transport Layer Protection ([OTG-CRYPST-001](https://www.owasp.org/index.php/Testing_for_Weak_SSL/TLS_Ciphers,_Insufficient_Transport_Layer_Protection_(OTG-CRYPST-001)))
*   *    Testing for Sensitive Information Sent via Unencrypted Channels
    *    Testing for Sensitive Information Sent via Unencrypted Channels ([OTG-CRYPST-003](https://www.owasp.org/index.php/Testing_for_Sensitive_information_sent_via_unencrypted_channels_(OTG-CRYPST-003)))
    *    Testing for Padding Oracle ([OTG-CRYPST-002](https://www.owasp.org/index.php/Testing_for_Padding_Oracle_(OTG-CRYPST-002)))
*   *    Storing Sensitive Information on Client Side
    *    Test Cross Origin Resource Sharing ([OTG-CLIENT-007](https://www.owasp.org/index.php/Test_Cross_Origin_Resource_Sharing_(OTG-CLIENT-007)))
    *    Test Local Storage ([OTG-CLIENT-012](https://www.owasp.org/index.php/Test_Local_Storage_(OTG-CLIENT-012)))
## Workflow/Dataflow Tests
*   *    Test Business Logic Data Validation ([OTG-BUSLOGIC-001](https://www.owasp.org/index.php/Test_business_logic_data_validation_(OTG-BUSLOGIC-001)))
    *    Test Ability to Forge Requests ([OTG-BUSLOGIC-002](https://www.owasp.org/index.php/Test_Ability_to_forge_requests_(OTG-BUSLOGIC-002)))
    *    Test Integrity Checks ([OTG-BUSLOGIC-003](https://www.owasp.org/index.php/Test_integrity_checks_(OTG-BUSLOGIC-003)))
    *    Test for Process Timing ([OTG-BUSLOGIC-004](https://www.owasp.org/index.php/Test_for_Process_Timing_(OTG-BUSLOGIC-004)))
    *    Test Number of Times a Function Can be Used Limits ([OTG-BUSLOGIC-005](https://www.owasp.org/index.php/Test_number_of_times_a_function_can_be_used_limits_(OTG-BUSLOGIC-005)))
    *    Testing for the Circumvention of Work Flows ([OTG-BUSLOGIC-006](https://www.owasp.org/index.php/Testing_for_the_Circumvention_of_Work_Flows_(OTG-BUSLOGIC-006)))
    *    Test Defenses Against Application Mis-use ([OTG-BUSLOGIC-007](https://www.owasp.org/index.php/Test_defenses_against_application_mis-use_(OTG-BUSLOGIC-007)))
