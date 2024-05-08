## Domain 2 - Asset security

- Asset security includes the concepts, structures, principles, and controls aimed at protecting assets—anything of value to the organization.
- Domain 2 gives an overview of the steps involved in asset security to address some of the issues that security professionals often encounter while implementing them.

#### Asset classification

- Asset classification policies, procedures, and processes help achieve proper protection of assets
- Protection of assets should always be based on the value of the asset.
- Proper asset classification ensures that assets receive an appropriate level of protection based on the value that they represent to the organization. Asset classification can be defined as assigning assets the level of protection they require, based on their value to the organization.

- Who is the owner of the asset? --> ultimately accountable for ensuring their assets are classified and thus protected appropriately

#### Information classification benefits
- Identification of critical information: identifies information that the organization considers critical to business success..
- Identification of sensitivity to modification: classification helps identify data that must only be modified in specifically authorized ways.
- Commitment to protect valuable assets: creates awareness among users that the organization is committed to protecting assets from unauthorized access.
- Commitment to confidentiality where applicable: classification helps ensure that sensitive information remains confidential.

#### Classification process
- Begins with a detailed asset inventory
- Asset owners determine the classification assigned to an asset
- Is an ongoing process
<p align="center">
  <img src="media/clasification_process.png?raw=true" alt="CIA triad"/>
</p>

| | Clasification vs Categorization| |
| --- | --- | --- |
| Clasification | System of classes ordered according to value | Top secret, secret, Company restricted, Proprietary,Personally Identifiable Information (PII)
| Categorization | The act of sorting into defined classifications

#### Labeling and marking
- Labeling refers to the classification of the asset and is system-readable
- Marking refers to the handling instructions of the asset and is human-readable
- Should be consistently applied to all assets within an organization
- Labeling should be cost-effective
  - Labeling methods: metadata, barcodes, qr, rfid, gps tags

#### Media handling
- Handling requirements are based on the classification of the asset, not the type of media    
- Owners determine who may access media, especially sensitive media
- Media Storage
  - top-secret data --> encrypted with robust algorithm (AES-256)

#### Data clasification policy
<p align="center">
  <img src="media/dcpolicy.png?raw=true" alt="CIA triad"/>
</p>

#### Information Life Cycle

<p align="center">
  <img src="media/dlcycle.png?raw=true" alt="CIA triad"/>
</p>

#### Data destruction 

<p align="center">
  <img src="media/destruction.png?raw=true" alt="CIA triad"/>
</p>

#### Data archiving
- Archiving/retention policy are based on laws, regulations, industry standards, and business needs
- Educate employees and provide them with the right tools

___

- Data at REST --> Inactive data that is stored on media
  - Protect --> encryption, access control, backup, and restoration
- Data in transit --> data that is moving across networks, like an organization’s internal network or the internet.
  - Protect --> 
    - end-to-end encryption --> End-to-end encryption means the data portion of a packet is encrypted immediately upon transmission from the source node, and the data remains encrypted through every node—every switch, router, firewall—through which it passes while traveling to the destination node
    - link encryption --> Link encryption means the packet header and data are encrypted between each node. Encrypting the packet header hides the routing information of packets traversing a network.
    - onion network
- Data in use --> data that is being used in some type of computational activity.
  - Protect --> homomorphic encryption, RBAC

___
 #### Information Obfuscation Methods
 - Concealing data --> Completely removes access to sensitive data. Users do not have access, nor do they have visibility and the attribute field does not appear on computer screens and reports.
 - Information Pruning/Pruning Data --> Information/Data pruning primarily takes place in nonproduction environments and involves the removal of sensitive data from attributes. The attribute will still be visible as a field on computer screens and reports, but it will not be populated with data.
 - Fabricating data --> Especially when testing the functionality of a system or in cases where particularly sensitive data exists, fabrication of data is often used.  
    1.   Creating fake data to replace real data facilitates full functional testing.  
    2.   Creating fake data to replace sensitive data prevents unauthorized access and viewing of the actual data.
 - Trimming data --> Removes part of an attribute’s value and is typically used for purposes of identification. Common examples of trimming involve Social Security numbers (SSN) and credit card numbers, where only the last four digits are visible and the remaining digits are masked.
 - Encrypting data --> Creates ciphertext of a value and can be done at the attribute, table, or database levels. With access to the proper key, encrypted data can be decrypted, and the ciphertext can be changed to plaintext. Like with trimming, credit card numbers are often encrypted when stored (for example, in a database) or when being transmitted.
___

- Digital Rights Management (DRM)
  - protects intellectual property (IP) assets and the rights of asset owners
  - Techniques
    - Licensing agreements that restrict access
    - Encryption
  - DRM technologies have primarily been used to protect mass-produced media such as songs and movies. The exact same techniques can be used to protect sensitive documents within an organization from unauthorized access and usage. This is referred to as Information Rights Management (IRM), a subset of DRM.

- Data Loss Prevention (DLP)
  - Data loss prevention focuses on the identification, monitoring, and protection of data.
  - DLP data activities take place in three contexts: data in use, data in motion, data at rest.