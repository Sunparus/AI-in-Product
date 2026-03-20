# System Architecture Documentation

## 1. Dependency Graph
- **REFERENCE_L0** is the foundation.
- **SKILL files** reference **REFERENCE_L0**.
- **Agent files** reference both **SKILL files** and **REFERENCE_L0**.
- **Evals** reference **SKILL files**.

## 2. Coupling Map
- **Critical Dependencies**: REFERENCE_L0 → SKILL files → Agent files  
- **Optional Dependencies**: Evals → SKILL files  
- **Potential Bottlenecks**: Over-reliance on REFERENCE_L0 could create bottlenecks if not managed properly.

## 3. Sync Checklist
- When **SKILL files** change, audit:  
    - **Agent files** for functionality  
    - **Evals** for consistency  
- When **REFERENCE_L0** changes, audit all dependents.

## 4. Future-Proof Branch Strategy
- Recommended: Only use **main branch** for simplicity.  
- Alternatively, utilize **feature branches** for SKILL development to manage larger updates independently.

## 5. Version Management
- Implement semantic versioning:  
    - Increment major version for breaking changes  
    - Increment minor version for feature additions  
    - Increment patch version for bug fixes  
- Update documentation whenever files are updated.

## 6. Circular Dependency Detection
- Regularly audit the dependency graph to ensure no circular references exist between files.

## 7. Breaking Change Protocol
- If **REFERENCE_L0** changes:  
    - Notify all teams of the breaking change.  
    - Schedule a timely update for all dependents to ensure consistency and compatibility.
    
- Document the changes and provide guidelines for the update process to each dependent file.  

---