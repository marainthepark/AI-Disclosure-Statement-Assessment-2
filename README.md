<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CACS304 Assessment 2 - AI Disclosure Statement</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
            line-height: 1.6;
            background-color: #f9f9f9;
        }
        .container {
            background: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        .header {
            text-align: center;
            margin-bottom: 30px;
            border-bottom: 2px solid #e0e0e0;
            padding-bottom: 20px;
        }
        .course-title {
            color: #d32f2f;
            font-size: 24px;
            font-weight: bold;
            margin: 0;
        }
        .assessment-title {
            color: #666;
            font-size: 18px;
            margin: 5px 0 0 0;
        }
        .section {
            margin-bottom: 25px;
        }
        .section-title {
            background-color: #f5f5f5;
            padding: 10px 15px;
            border-left: 4px solid #d32f2f;
            margin-bottom: 15px;
            font-weight: bold;
            color: #333;
        }
        .form-group {
            margin-bottom: 20px;
        }
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: #333;
        }
        input[type="text"], input[type="url"], textarea, select {
            width: 100%;
            padding: 12px;
            border: 2px solid #ddd;
            border-radius: 4px;
            font-size: 14px;
            box-sizing: border-box;
            transition: border-color 0.3s;
        }
        input[type="text"]:focus, input[type="url"]:focus, textarea:focus, select:focus {
            outline: none;
            border-color: #d32f2f;
        }
        textarea {
            resize: vertical;
            min-height: 100px;
        }
        .checkbox-group {
            margin: 15px 0;
        }
        .checkbox-group input[type="checkbox"] {
            width: auto;
            margin-right: 10px;
        }
        .checkbox-group label {
            display: inline;
            font-weight: normal;
        }
        .help-text {
            font-size: 12px;
            color: #666;
            font-style: italic;
            margin-top: 5px;
        }
        .button-group {
            text-align: center;
            margin-top: 30px;
            padding-top: 20px;
            border-top: 1px solid #e0e0e0;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 10px;
        }
        .btn {
            background-color: #d32f2f;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 14px;
            transition: background-color 0.3s;
            white-space: nowrap;
            flex-shrink: 0;
        }
        .btn:hover {
            background-color: #b71c1c;
        }
        .btn-secondary {
            background-color: #666;
        }
        .btn-secondary:hover {
            background-color: #555;
        }
        .required {
            color: #d32f2f;
        }
        .submission-info {
            margin-top: 15px;
            padding: 15px;
            background-color: #e8f5e8;
            border-radius: 4px;
            border-left: 4px solid #4caf50;
        }
        .research-tools-note {
            background-color: #fff3e0;
            border: 1px solid #ffb74d;
            border-radius: 4px;
            padding: 15px;
            margin: 15px 0;
        }
        .research-tools-note strong {
            color: #f57c00;
        }
        @media print {
            body { background-color: white; }
            .container { box-shadow: none; }
            .button-group { display: none; }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1 class="course-title">CACS304: Creative Research</h1>
            <h2 class="assessment-title">Assessment 2: Literature/Contextual Review<br>AI Disclosure Statement</h2>
        </div>

        <form id="aiDisclosureForm">
            <div class="section">
                <div class="form-group">
                    <label for="studentName">Student Name: <span class="required">*</span></label>
                    <input type="text" id="studentName" name="studentName" required>
                </div>
                
                <div class="form-group">
                    <label for="studentId">Student ID: <span class="required">*</span></label>
                    <input type="text" id="studentId" name="studentId" required>
                </div>
            </div>

            <div class="section">
                <div class="section-title">AI Tool Usage Declaration</div>
                
                <div class="checkbox-group">
                    <input type="checkbox" id="noAiUsed" name="aiUsage" value="none">
                    <label for="noAiUsed">I did not use any AI tools in the preparation of this assessment</label>
                </div>
                
                <div class="checkbox-group">
                    <input type="checkbox" id="aiUsed" name="aiUsage" value="used">
                    <label for="aiUsed">I used AI tools in the preparation of this assessment (complete sections below)</label>
                </div>
            </div>

            <div id="aiDetailsSection" style="display: none;">
                <div class="section">
                    <div class="section-title">AI Tools Used</div>
                    
                    <div class="research-tools-note">
                        <strong>Research Tools:</strong> You may have been introduced to specialised research AI tools. These can be useful additions to your research toolkit but will not find all the sources you need for creative arts research.
                    </div>
                    
                    <div class="form-group">
                        <label>Which AI system(s) did you use? (Select all that apply) <span class="required">*</span></label>
                        
                        <strong style="color: #666; font-size: 14px; margin-top: 10px; display: block;">General AI Tools:</strong>
                        <div class="checkbox-group">
                            <input type="checkbox" id="chatgpt" name="aiSystems" value="ChatGPT">
                            <label for="chatgpt">ChatGPT (OpenAI)</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="claude" name="aiSystems" value="Claude">
                            <label for="claude">Claude (Anthropic)</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="gemini" name="aiSystems" value="Gemini">
                            <label for="gemini">Google Gemini (formerly Bard)</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="copilot" name="aiSystems" value="Copilot">
                            <label for="copilot">Microsoft Copilot</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="grammarly" name="aiSystems" value="Grammarly">
                            <label for="grammarly">Grammarly AI</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="notion" name="aiSystems" value="Notion AI">
                            <label for="notion">Notion AI</label>
                        </div>
                        
                        <strong style="color: #666; font-size: 14px; margin-top: 15px; display: block;">Research-Specific AI Tools:</strong>
                        <div class="checkbox-group">
                            <input type="checkbox" id="scholarcy" name="aiSystems" value="Scholarcy">
                            <label for="scholarcy">Scholarcy (paper summarisation)</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="elicit" name="aiSystems" value="Elicit">
                            <label for="elicit">Elicit (research question answering)</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="consensus" name="aiSystems" value="Consensus">
                            <label for="consensus">Consensus (research synthesis)</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="research-rabbit" name="aiSystems" value="Research Rabbit">
                            <label for="research-rabbit">Research Rabbit (source discovery)</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="perplexity" name="aiSystems" value="Perplexity">
                            <label for="perplexity">Perplexity AI (AI search engine)</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="other-ai" name="aiSystems" value="Other">
                            <label for="other-ai">Other (specify below)</label>
                        </div>
                        <input type="text" id="otherAiSpecify" name="otherAiSpecify" placeholder="If 'Other', please specify which AI tool(s)" style="margin-top: 10px;">
                    </div>
                </div>

                <div class="section">
                    <div class="section-title">How You Used AI</div>
                    
                    <div class="form-group">
                        <label>Which aspects of your literature review did you use AI for? (Select all that apply)</label>
                        <div class="checkbox-group">
                            <input type="checkbox" id="use-source-discovery" name="aiUses" value="source-discovery">
                            <label for="use-source-discovery">Source discovery and searching</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="use-reading" name="aiUses" value="reading-comprehension">
                            <label for="use-reading">Reading and understanding complex academic texts</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="use-analyzing" name="aiUses" value="analyzing-summarizing">
                            <label for="use-analyzing">Analysing and summarising sources</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="use-organizing" name="aiUses" value="organizing-sources">
                            <label for="use-organizing">Organising sources into categories</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="use-themes" name="aiUses" value="identifying-themes">
                            <label for="use-themes">Identifying themes and patterns in literature</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="use-introduction" name="aiUses" value="writing-introduction">
                            <label for="use-introduction">Writing the literature review introduction</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="use-body" name="aiUses" value="writing-body">
                            <label for="use-body">Writing the literature review body</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="use-conclusion" name="aiUses" value="writing-conclusion">
                            <label for="use-conclusion">Writing the literature review conclusion</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="use-visual-maps" name="aiUses" value="visual-organization">
                            <label for="use-visual-maps">Creating visual maps/organisation tools</label>
                        </div>
                        <div class="checkbox-group">
                            <input type="checkbox" id="use-writing-editing" name="aiUses" value="writing-editing">
                            <label for="use-writing-editing">General writing assistance and editing</label>
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label for="specificSections">Provide specific details about how you used AI for the aspects you selected above:</label>
                        <textarea id="specificSections" name="specificSections" placeholder="For each aspect you ticked above, explain specifically how you used AI. For example:

Source discovery: Used Research Rabbit to find additional sources related to my chosen practitioner after initial library searches.

Analysing sources: Used Claude to help break down complex theoretical arguments in academic papers to better understand the key concepts.

Writing assistance: Used Grammarly to check grammar and clarity throughout the literature review."></textarea>
                        <div class="help-text">Be specific about how AI helped with each aspect you selected</div>
                    </div>
                </div>

                <div class="section">
                    <div class="section-title">Examples of Prompts Used</div>
                    
                    <div class="form-group">
                        <label for="prompts">Give an example of the kind of prompts that you used:</label>
                        <textarea id="prompts" name="prompts" placeholder="Provide 1-2 examples of the types of prompts you used with AI tools. You don't need to list every single prompt.

Example:
'Can you help me identify the main themes in this literature about contemporary dance pedagogy? Here are the key sources I've found: [list of sources]'

'I'm writing a literature review about site-specific performance. Can you help me organise these sources into logical categories based on their approaches to space and place?'"></textarea>
                        <div class="help-text">Focus on giving representative examples rather than listing every prompt you used</div>
                    </div>
                </div>

                <div class="section">
                    <div class="section-title">How AI Output Was Used</div>
                    
                    <div class="form-group">
                        <label for="outputUse">How did you incorporate the AI output into your final literature review?</label>
                        <textarea id="outputUse" name="outputUse" placeholder="Explain how you used the AI suggestions in your final submission. Did you use text directly, modify suggestions, or use ideas as starting points? Be specific about how AI contributions were integrated into your literature review."></textarea>
                    </div>
                </div>

                <div class="section">
                    <div class="section-title">Value of AI Tool</div>
                    
                    <div class="form-group">
                        <label for="aiValue">What value did this AI tool offer during your literature review preparation?</label>
                        <textarea id="aiValue" name="aiValue" placeholder="Reflect on how the AI tool helped your research and writing process. What did it enable you to do that you might not have done otherwise? How did it support your understanding of the literature in your field?"></textarea>
                    </div>
                </div>
            </div>

            <div class="button-group">
                <button type="button" class="btn btn-secondary" onclick="clearForm()">Clear Form</button>
                <button type="button" class="btn" onclick="downloadPDF()">Download as PDF</button>
                <button type="button" class="btn btn-secondary" onclick="downloadText()">Download as Text</button>
                <button type="button" class="btn btn-secondary" onclick="copyToClipboard()">Copy to Clipboard</button>
            </div>
            
            <div class="submission-info">
                <strong>📁 How to Submit:</strong> Click "Download as PDF" to save your AI disclosure statement, then upload this PDF file to FeedbackFruits along with your literature review document.
            </div>
        </form>
    </div>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
    <script>
        // Show/hide AI details section based on checkbox selection
        document.querySelectorAll('input[name="aiUsage"]').forEach(checkbox => {
            checkbox.addEventListener('change', function() {
                const aiDetailsSection = document.getElementById('aiDetailsSection');
                const aiUsedCheckbox = document.getElementById('aiUsed');
                
                if (aiUsedCheckbox.checked) {
                    aiDetailsSection.style.display = 'block';
                    // Make required fields required
                    document.getElementById('prompts').required = true;
                } else {
                    aiDetailsSection.style.display = 'none';
                    // Remove required attribute
                    document.getElementById('prompts').required = false;
                }
                
                // Ensure only one checkbox is selected
                document.querySelectorAll('input[name="aiUsage"]').forEach(cb => {
                    if (cb !== this) cb.checked = false;
                });
            });
        });

        function clearForm() {
            if (confirm('Are you sure you want to clear all form data?')) {
                document.getElementById('aiDisclosureForm').reset();
                document.getElementById('aiDetailsSection').style.display = 'none';
                document.getElementById('prompts').required = false;
            }
        }

        // Download submission file as PDF
        function downloadPDF() {
            console.log('PDF download clicked');
            
            if (!validateForm()) {
                console.log('Validation failed');
                return;
            }
            
            console.log('Validation passed, generating PDF');
            
            try {
                const { jsPDF } = window.jspdf;
                const doc = new jsPDF();
                
                const studentName = document.getElementById('studentName').value;
                const studentId = document.getElementById('studentId').value;
                const aiUsage = document.querySelector('input[name="aiUsage"]:checked')?.value;
                
                // Colors
                const primaryColor = [211, 47, 47]; // UOW red
                const textColor = [51, 51, 51]; // Dark grey
                const lightGrey = [128, 128, 128];
                
                // Header section with university branding
                doc.setFillColor(primaryColor[0], primaryColor[1], primaryColor[2]);
                doc.rect(0, 0, 210, 35, 'F');
                
                doc.setTextColor(255, 255, 255);
                doc.setFontSize(20);
                doc.setFont(undefined, 'bold');
                doc.text('CACS304: Creative Research', 20, 15);
                
                doc.setFontSize(14);
                doc.setFont(undefined, 'normal');
                doc.text('Assessment 2: Literature/Contextual Review', 20, 23);
                doc.text('AI Disclosure Statement', 20, 30);
                
                // Student info box
                doc.setFillColor(248, 248, 248);
                doc.rect(15, 45, 180, 25, 'F');
                doc.setDrawColor(200, 200, 200);
                doc.rect(15, 45, 180, 25, 'S');
                
                doc.setTextColor(textColor[0], textColor[1], textColor[2]);
                doc.setFontSize(12);
                doc.setFont(undefined, 'bold');
                doc.text('Student Information', 20, 53);
                
                doc.setFont(undefined, 'normal');
                doc.setFontSize(10);
                doc.text(`Name: ${studentName}`, 20, 60);
                doc.text(`Student ID: ${studentId}`, 20, 65);
                doc.text(`Date: ${new Date().toLocaleDateString('en-AU')}`, 120, 60);
                doc.text(`Assessment: Literature/Contextual Review`, 120, 65);
                
                let yPosition = 85;
                
                if (aiUsage === 'none') {
                    // No AI used section
                    doc.setFillColor(232, 245, 233);
                    doc.rect(15, yPosition, 180, 30, 'F');
                    doc.setDrawColor(76, 175, 80);
                    doc.setLineWidth(2);
                    doc.line(15, yPosition, 15, yPosition + 30);
                    
                    doc.setTextColor(textColor[0], textColor[1], textColor[2]);
                    doc.setFontSize(14);
                    doc.setFont(undefined, 'bold');
                    doc.text('AI Usage Declaration', 20, yPosition + 8);
                    
                    doc.setFontSize(11);
                    doc.setFont(undefined, 'normal');
                    const noAiText = doc.splitTextToSize('I did not use any AI tools in the preparation of this literature review assessment.', 170);
                    doc.text(noAiText, 20, yPosition + 18);
                    
                } else {
                    // AI used section
                    const aiSystems = Array.from(document.querySelectorAll('input[name="aiSystems"]:checked')).map(cb => cb.value);
                    const otherAiSpecify = document.getElementById('otherAiSpecify')?.value || '';
                    const aiUses = Array.from(document.querySelectorAll('input[name="aiUses"]:checked')).map(cb => cb.value);
                    const specificSections = document.getElementById('specificSections')?.value || '';
                    const prompts = document.getElementById('prompts')?.value || '';
                    const outputUse = document.getElementById('outputUse')?.value || '';
                    const aiValue = document.getElementById('aiValue')?.value || '';

                    let systemsList = aiSystems.join(', ');
                    if (aiSystems.includes('Other') && otherAiSpecify) {
                        systemsList = systemsList.replace('Other', otherAiSpecify);
                    }

                    let usesList = aiUses.map(use => getUseDescription(use)).join(', ');

                    // AI Declaration header
                    doc.setFillColor(255, 245, 238);
                    doc.rect(15, yPosition, 180, 15, 'F');
                    doc.setDrawColor(255, 152, 0);
                    doc.setLineWidth(2);
                    doc.line(15, yPosition, 15, yPosition + 15);
                    
                    doc.setTextColor(textColor[0], textColor[1], textColor[2]);
                    doc.setFontSize(14);
                    doc.setFont(undefined, 'bold');
                    doc.text('AI Usage Declaration', 20, yPosition + 8);
                    
                    yPosition += 25;
                    
                    // Declaration text
                    doc.setFontSize(11);
                    doc.setFont(undefined, 'normal');
                    const declarationText = `I acknowledge the use of ${systemsList} for assistance with the following aspects of my literature review: ${usesList}.`;
                    const splitDeclaration = doc.splitTextToSize(declarationText, 170);
                    doc.text(splitDeclaration, 20, yPosition);
                    yPosition += splitDeclaration.length * 5 + 15;
                    
                    // Helper function to add sections
                    function addSection(title, content, startY) {
                        if (!content || content.trim() === '') return startY;
                        
                        // Section header
                        doc.setFillColor(250, 250, 250);
                        doc.rect(15, startY, 180, 8, 'F');
                        doc.setTextColor(primaryColor[0], primaryColor[1], primaryColor[2]);
                        doc.setFontSize(11);
                        doc.setFont(undefined, 'bold');
                        doc.text(title, 20, startY + 5);
                        
                        startY += 12;
                        
                        // Content
                        doc.setTextColor(textColor[0], textColor[1], textColor[2]);
                        doc.setFontSize(10);
                        doc.setFont(undefined, 'normal');
                        const splitContent = doc.splitTextToSize(content, 170);
                        
                        splitContent.forEach(line => {
                            if (startY > 270) {
                                doc.addPage();
                                startY = 20;
                            }
                            doc.text(line, 20, startY);
                            startY += 5;
                        });
                        
                        return startY + 10;
                    }
                    
                    // Add all sections
                    yPosition = addSection('Specific Use by Aspect:', specificSections, yPosition);
                    yPosition = addSection('Examples of Prompts Used:', prompts, yPosition);
                    yPosition = addSection('How AI Output Was Used:', outputUse, yPosition);
                    yPosition = addSection('Value of AI Tool:', aiValue, yPosition);
                    
                    // Confirmation statement
                    if (yPosition > 240) {
                        doc.addPage();
                        yPosition = 20;
                    }
                    
                    doc.setFillColor(240, 248, 255);
                    const confirmHeight = 25;
                    doc.rect(15, yPosition, 180, confirmHeight, 'F');
                    doc.setDrawColor(33, 150, 243);
                    doc.setLineWidth(1);
                    doc.rect(15, yPosition, 180, confirmHeight, 'S');
                    
                    doc.setTextColor(textColor[0], textColor[1], textColor[2]);
                    doc.setFontSize(10);
                    doc.setFont(undefined, 'italic');
                    const confirmText = 'I confirm that the final literature review is my own work and represents my personal analysis and understanding of the academic literature in my field. While I used AI assistance as described above, all critical analysis, arguments, and written expression in the final submission are my own. I used AI tools responsibly to support my research and writing process, not to replace my own scholarly thinking and analysis.';
                    const splitConfirm = doc.splitTextToSize(confirmText, 170);
                    doc.text(splitConfirm, 20, yPosition + 6);
                }
                
                // Footer
                const pageCount = doc.internal.getNumberOfPages();
                for (let i = 1; i <= pageCount; i++) {
                    doc.setPage(i);
                    doc.setTextColor(lightGrey[0], lightGrey[1], lightGrey[2]);
                    doc.setFontSize(8);
                    doc.setFont(undefined, 'normal');
                    doc.text(`Generated: ${new Date().toLocaleString('en-AU')}`, 20, 290);
                    doc.text(`Page ${i} of ${pageCount}`, 170, 290);
                }
                
                // Generate filename and save
                const filename = `${studentId}_${studentName.replace(/\s+/g, '_')}_AI_Disclosure_Assessment2.pdf`;
                doc.save(filename);
                
                // Show success message
                setTimeout(() => {
                    alert('✅ AI Disclosure Statement downloaded as PDF!\n\nPlease upload this PDF file to FeedbackFruits along with your literature review.');
                }, 100);
                
            } catch (error) {
                console.error('PDF generation error:', error);
                alert('Error generating PDF. Please try the "Download as Text" option instead, or contact your instructor.');
            }
        }

        // Download submission file as text (backup option)
        function downloadText() {
            console.log('Text download clicked');
            
            if (!validateForm()) {
                console.log('Validation failed');
                return;
            }
            
            console.log('Validation passed, generating text file');
            
            try {
                const formattedData = generateSubmissionText();
                const studentName = document.getElementById('studentName').value;
                const studentId = document.getElementById('studentId').value;
                
                // Create downloadable text file
                const blob = new Blob([formattedData], { type: 'text/plain;charset=utf-8' });
                const url = window.URL.createObjectURL(blob);
                const a = document.createElement('a');
                a.href = url;
                a.download = `${studentId}_${studentName.replace(/\s+/g, '_')}_AI_Disclosure_Assessment2.txt`;
                document.body.appendChild(a);
                a.click();
                document.body.removeChild(a);
                window.URL.revokeObjectURL(url);
                
                // Show success message
                setTimeout(() => {
                    alert('✅ AI Disclosure Statement downloaded as text file!\n\nPlease upload this file to FeedbackFruits along with your literature review.');
                }, 100);
                
            } catch (error) {
                console.error('Text download error:', error);
                alert('Error generating text file. Please contact your instructor.');
            }
        }

        // Copy formatted submission to clipboard
        async function copyToClipboard() {
            console.log('Copy to clipboard clicked');
            
            if (!validateForm()) {
                console.log('Validation failed');
                return;
            }
            
            console.log('Validation passed, copying to clipboard');
            
            try {
                const formattedData = generateSubmissionText();
                
                try {
                    await navigator.clipboard.writeText(formattedData);
                    alert('AI Disclosure Statement copied to clipboard! You can now paste it into an email or your LMS submission.');
                } catch (err) {
                    // Fallback for older browsers
                    const textArea = document.createElement('textarea');
                    textArea.value = formattedData;
                    document.body.appendChild(textArea);
                    textArea.select();
                    document.execCommand('copy');
                    document.body.removeChild(textArea);
                    alert('AI Disclosure Statement copied to clipboard! You can now paste it into an email or your LMS submission.');
                }
                
            } catch (error) {
                console.error('Copy to clipboard error:', error);
                alert('Error copying to clipboard. Please try the download options instead.');
            }
        }

        // Validate required fields
        function validateForm() {
            const studentName = document.getElementById('studentName').value;
            const studentId = document.getElementById('studentId').value;
            const aiUsageChecked = document.querySelector('input[name="aiUsage"]:checked');
            
            if (!studentName) {
                alert('Please enter your name.');
                document.getElementById('studentName').focus();
                return false;
            }
            
            if (!studentId) {
                alert('Please enter your student ID.');
                document.getElementById('studentId').focus();
                return false;
            }
            
            if (!aiUsageChecked) {
                alert('Please indicate whether you used AI tools or not.');
                return false;
            }
            
            // If AI was used, check required fields
            if (aiUsageChecked.value === 'used') {
                const aiSystemsChecked = document.querySelectorAll('input[name="aiSystems"]:checked');
                const prompts = document.getElementById('prompts').value;
                
                if (aiSystemsChecked.length === 0) {
                    alert('Please select which AI system(s) you used.');
                    return false;
                }
                
                if (!prompts.trim()) {
                    alert('Please provide an example of the kind of prompts you used with AI tools.');
                    document.getElementById('prompts').focus();
                    return false;
                }
                
                // Check if at least one use case is selected
                const aiUsesChecked = document.querySelectorAll('input[name="aiUses"]:checked');
                if (aiUsesChecked.length === 0) {
                    alert('Please select which aspects of your literature review you used AI for.');
                    return false;
                }
                
                // Check if specific sections field is filled
                const specificSections = document.getElementById('specificSections').value;
                if (!specificSections.trim()) {
                    alert('Please provide specific details about how you used AI for the aspects you selected.');
                    document.getElementById('specificSections').focus();
                    return false;
                }
            }
            
            return true;
        }

        // Generate formatted submission text for display
        function generateSubmissionText() {
            const studentName = document.getElementById('studentName').value || '';
            const studentId = document.getElementById('studentId').value || '';
            const aiUsage = document.querySelector('input[name="aiUsage"]:checked')?.value || '';
            
            let submission = `CACS304: Creative Research - Assessment 2 Literature/Contextual Review
AI DISCLOSURE STATEMENT
================================================================

Student Name: ${studentName}
Student ID: ${studentId}
Date: ${new Date().toLocaleDateString('en-AU')}
Assessment: Literature/Contextual Review

================================================================

`;

            if (aiUsage === 'none') {
                submission += `AI USAGE DECLARATION:

I did not use any AI tools in the preparation of this literature review assessment.

================================================================

This statement confirms that my literature review, including source discovery, analysis, organisation, and written expression, was completed without the assistance of artificial intelligence tools.`;
            } else {
                const aiSystems = Array.from(document.querySelectorAll('input[name="aiSystems"]:checked')).map(cb => cb.value);
                const otherAiSpecify = document.getElementById('otherAiSpecify')?.value || '';
                const aiUses = Array.from(document.querySelectorAll('input[name="aiUses"]:checked')).map(cb => cb.value);
                const specificSections = document.getElementById('specificSections')?.value || '';
                const prompts = document.getElementById('prompts')?.value || '';
                const outputUse = document.getElementById('outputUse')?.value || '';
                const aiValue = document.getElementById('aiValue')?.value || '';

                let systemsList = aiSystems.join(', ');
                if (aiSystems.includes('Other') && otherAiSpecify) {
                    systemsList = systemsList.replace('Other', otherAiSpecify);
                }

                let usesList = aiUses.map(use => getUseDescription(use)).join(', ');

                submission += `AI USAGE DECLARATION:

I acknowledge the use of ${systemsList} for assistance with the following aspects of my literature review: ${usesList}.

================================================================

SPECIFIC USE BY ASPECT:
${specificSections}

================================================================

EXAMPLES OF PROMPTS USED:
${prompts}

================================================================

HOW AI OUTPUT WAS USED IN MY LITERATURE REVIEW:
${outputUse}

================================================================

VALUE OF AI TOOL IN MY RESEARCH PROCESS:
${aiValue}

================================================================

I confirm that the final literature review is my own work and represents my personal analysis and understanding of the academic literature in my field. While I used AI assistance as described above, all critical analysis, arguments, and written expression in the final submission are my own. I used AI tools responsibly to support my research and writing process, not to replace my own scholarly thinking and analysis.`;
            }

            submission += `

================================================================
Generated: ${new Date().toLocaleString('en-AU')}
Form completed at: ${window.location.href}`;

            return submission;
        }

        // Convert use selections to descriptions
        function getUseDescription(use) {
            const descriptions = {
                'source-discovery': 'Source discovery and searching',
                'reading-comprehension': 'Reading and understanding complex academic texts',
                'analyzing-summarizing': 'Analysing and summarising sources',
                'organizing-sources': 'Organising sources into categories',
                'identifying-themes': 'Identifying themes and patterns in literature',
                'writing-introduction': 'Writing the literature review introduction',
                'writing-body': 'Writing the literature review body',
                'writing-conclusion': 'Writing the literature review conclusion',
                'visual-organization': 'Creating visual maps/organisation tools',
                'writing-editing': 'General writing assistance and editing'
            };
            return descriptions[use] || use;
        }

        // Auto-save to localStorage (optional)
        function saveFormData() {
            const formData = new FormData(document.getElementById('aiDisclosureForm'));
            const data = Object.fromEntries(formData);
            localStorage.setItem('cacs304_ai_disclosure_assessment2', JSON.stringify(data));
        }

        // Auto-save every 30 seconds
        setInterval(saveFormData, 30000);

        // Load saved data on page load
        window.addEventListener('load', function() {
            const savedData = localStorage.getItem('cacs304_ai_disclosure_assessment2');
            if (savedData) {
                const data = JSON.parse(savedData);
                Object.keys(data).forEach(key => {
                    const element = document.getElementById(key);
                    if (element) {
                        if (element.type === 'checkbox') {
                            element.checked = data[key] === element.value;
                        } else {
                            element.value = data[key];
                        }
                    }
                });
                // Trigger the AI usage display logic
                if (data.aiUsage === 'used') {
                    document.getElementById('aiUsed').checked = true;
                    document.getElementById('aiDetailsSection').style.display = 'block';
                    document.getElementById('prompts').required = true;
                }
            }
        });
    </script>
</body>
</html>
