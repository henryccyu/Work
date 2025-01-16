# Risk Engine - Risk Register Integration Discussion

## Summary of Discussion Points and Action Items
### Priority Stack for Necessary Operations
#### Priority 0: Risk Creation
- Develop necessary APIs and processes to support the creation of risks within the system.  
- User access management: Define roles, permissions, and processes for managing system access to the API and related systems.
#### Priority 1: State Management
- Define and implement necessary APIs and processes for managing the state of risks within the system.  
- Authentication and Authorization: Risk Engine will use managed identities to authenticate. There are two ways of provisioning the RiskEngine identity:
  1. Create an ADO Work Item for Risk Register and let a DRI run scripts to provision the access.
  2. Follow SpaceTool steps to submit an admin consent request.

### Risk Creation and Data Contracts
- Risk Engine will send new additional parameters to track the origin of a Risk:
  1. Source: Risk Engine
  2. Source Id: The Id of the Risk Archetype.
  3. Source Unique Id: The Id of the Risk at the source, which uniquely identifies the Risk at its source.

### Action Items
- Define Data Contract: Risk Engine team to work on a data contract and SLA’s for the new API. The Risk register team will review the current API to determine if it can be used with modifications or if a new API needs to be created.  
- Provisioning Managed Identity: Request admin consent through the space tool using the provided app IDs.

### Open Ended Items
- Define the system’s state transitioning when User makes changes through UI and Risk engine making changes through API to ensure consistency and avoid conflicts.  
- Determine if Risk Register should store additional Risk Archetype metadata apart from RiskArcheTypeID Guid for reporting purposes.

### Next Steps
- A follow-up meeting will be set up once there is some data on the action items to discuss the Data Contract part further.
