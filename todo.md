```markdown
### Core
[ ] 1. Define core question bank and types  
**Validation**: Type-check passes for sample questions in lib/questions.ts  
[ ] 2. Implement state initialization logic  
**Validation**: POST /start creates valid state object with session ID  
[ ] 3. Setup question progression logic  
**Validation**: State correctly advances to next question index  
[ ] 4. Add score calculation utilities  
**Validation**: Correct answers increment score in test cases  
[ ] 5. Create state validation middleware  
**Validation**: Invalid state triggers error recovery flow  
[ ] 6. Implement URL param encryption  
**Validation**: Encrypted params survive round-trip decryption  
[ ] 7. Add session timeout detection  
**Validation**: 24h old sessions get expired automatically  

### API
[ ] 1. Create base API route structure  
**Validation**: /api/frame returns 200 with empty response  
[ ] 2. Implement root GET frame endpoint  
**Validation**: GET /api/frame returns valid frame metadata  
[ ] 3. Build /start POST handler  
**Validation**: POST to /start returns 302 redirect to first question  
[ ] 4. Create /question POST endpoint  
**Validation**: Valid requests return question frame with 4 buttons  
[ ] 5. Implement /answer processing endpoint  
**Validation**: Correct answers show ✓, incorrect shows ✗ in testing  
[ ] 6. Add /results endpoint  
**Validation**: Final redirect shows total score/10 in metadata  
[ ] 7. Create /restart endpoint  
**Validation**: New session ID generated on restart request  

### UI
[ ] 1. Create FrameButton component  
**Validation**: Renders clickable buttons with target URLs  
[ ] 2. Build welcome frame SVG generator  
**Validation**: Displays "Start Quiz" button in frame preview  
[ ] 3. Implement question template system  
**Validation**: Shows different questions with randomized button order  
[ ] 4. Create progress indicator component  
**Validation**: Displays "Question 3/10" in test frames  
[ ] 5. Build score visualization overlay  
**Validation**: Current score updates after each answer  
[ ] 6. Design results frame template  
**Validation**: Shows final score and trophy emoji for >80%  
[ ] 7. Implement error state frames  
**Validation**: Invalid requests show "Session expired" message  
[ ] 8. Add hover animations to buttons  
**Validation**: Buttons scale 10% on hover in desktop view  
```

Tasks ordered by implementation dependencies within each category. Core foundation established first, followed by API endpoints and UI components in parallel. Validation criteria ensure each feature works in isolation before integration.