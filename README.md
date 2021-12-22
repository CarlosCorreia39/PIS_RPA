# Specification-based on Use Cases Scenarios

DataEntities: 

DataEntity e_backOfficeOperator is a Master […].  

DataEntity e_organizationalEntity is a Master […].  

DataEntity e_document is a Document […].  

 

Actors: 

Actor a_backOfficeOperator (Operator) is a User who Process documents. 

Actor a_OrganizationalEntity (Customer) is a User, who creates documents. 

Actor, a_Robot (Robot), is the robot responsible for robotic process automation. 

 

Use Cases: 

UseCase uc_3_SoftRobot is a EntitiesManage with e_document, actor_a_Robot. 

Spec. 6: Specification-based on Use Cases (uc_3_SoftRobot) 

 

Use Cases Scenarios: 

 

UseCase uc_3_SoftRobot 

[…] 

Scenario MainScenario (Main): 

Robot: Get from a specific location folder the list of digitalized documents (in a “pdf” format), with file names outside the standard format. 

Robot: Read and convert each document from “pdf” into “txt” format, using OCR technology with a scale of zero. 

Robot: Browses the list of Documents and opens each one of them in “txt” format. 

Robot: For each document, extract and insert in an excel file the following text fragments: document type, organizational entity (responsible for document creation), process number and creation year.  

Robot: In addiction, insert into the excel file the path where the document is located. 

Robot: Get the document filename in the correct standard format from the Excel file and change the filename of each one. 

Robot: If the document filename is in the correct format then upload the file into the data store of the SICMAR application and move it to the Processed Document Folder.  

Robot: In case the document file has an incorrect format filename then move it to the Failed Document Folder. 

Robot: Send an email message to the IT Manager specifying how many and which documents have already been successfully inserted into the system and how many and which have failed. 


# Specification based on Pseudocode
