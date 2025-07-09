# flowchat
a flowchat for surf
graph TD
    A[User asks a question in the forum] --> B{AI Agent analyzes the question};
    B --> C{Instructor is notified & can choose to answer directly};
    C --> D[Instructor posts answer];
    B --> E{AI searches database for context};
    E --> F[Presents relevant context to instructor];
    F --> G{Instructor selects context & provides instructions};
    G --> H[AI drafts a response];
    H --> I{Instructor reviews, edits, and approves};
    I --> J[AI posts the approved answer];
    H --> K{Engage in Critical Reflection};
    K --> L[Challenge AI/group assumptions];
    L --> H;

    subgraph "Instructor Loop"
        C; D; F; G; I; J;
    end

    subgraph "Critical Thinking Loop"
        K; L;
    end

    style A fill:#D6EAF8,stroke:#333,stroke-width:2px
    style B fill:#E8DAEF,stroke:#333,stroke-width:2px
    style E fill:#E8DAEF,stroke:#333,stroke-width:2px
    style H fill:#E8DAEF,stroke:#333,stroke-width:2px
    style K fill:#FAD7A0,stroke:#333,stroke-width:2px
    style L fill:#FAD7A0,stroke:#333,stroke-width:2px
