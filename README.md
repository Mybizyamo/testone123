rag-agent-app/
│
├── data/                         
│   ├── raw/                      
│   └── processed/                
│
├── embeddings/                  
│   ├── generateEmbeddings.js     
│   └── vectorStore/              
│
├── retriever/                   
│   └── retriever.js              
│
├── agent/                        # Core agent logic
│   ├── AgentOrchestrator.js      # Main agent class: plans, calls tools, builds prompt
│   ├── ToolRegistry.js           # Registry of callable tools
│   ├── tools/                    # Available agent tools
│   │   ├── summarize.js          
│   │   ├── calculator.js         
│   │   └── search.js             
│   ├── MemoryStore.js            # Optional: in-memory or Redis-based memory
│   └── PlanGenerator.js          # Optional: breaks task into substeps
│
├── llm/                         
│   ├── llmClient.js              
│   └── promptTemplates.js        
│
├── server/                      
│   └── index.js                  
│
├── config/                      
│   └── config.js                 
│
├── utils/                       
│   └── helpers.js                
│
├── test/                        
│   └── agent.test.js             
│
├── .env                          
├── package.json                 
└── README.md                    
