# PromptLab
Colección personal de prompts para IA, organizados para facilitar su reutilización y experimentación.

# Edu-management

## Encuadres pedagógicos

Con nivel de Ph.D. en Pedagogía escribe un encuadre pedagógico para la institución educativa [IE], el grado [GRADO] en el área de [ÁREA]. Debe estar diseñado para el [NÚMERO] periodo académico, abarcando aproximadamente [NÚMERO] semanas a partir de [FECHA INICIAL]. 

El encuadre debe incluir:

**1. SABER:**  
- Describir los aprendizajes conceptuales que el estudiante debe adquirir (usando el infinitivo). 
  - Ejemplo: "Comprender los conceptos fundamentales de..."

**2. HACER:**  
- Describir las habilidades prácticas y competencias que se espera que el estudiante desarrolle (usando el infinitivo). 
  - Ejemplo: "Aplicar técnicas de..."

**3. SER:**  
- Describir las actitudes, valores y aspectos formativos que se busca fomentar en el estudiante (usando el infinitivo). 
  - Ejemplo: "Fomentar la responsabilidad en..."

**4. CRITERIOS DE EVALUACIÓN:**  
- Establecer los criterios que se utilizarán para evaluar el desempeño del estudiante, detallando los indicadores claros y medibles.
  - Ejemplo: "Evaluar la capacidad de..."

**5. RESULTADOS DE APRENDIZAJE:**  
- Redactar los resultados de aprendizaje esperados de manera precisa y medible.
  - Ejemplo: "El estudiante será capaz de..."

**6. EVIDENCIAS DE APRENDIZAJE:**  
- Identificar las evidencias que el estudiante debe presentar para demostrar el logro de los aprendizajes.
  - Ejemplo: "Presentar un informe sobre..."

**7. POSIBLES FECHAS:**  
- Sugerir fechas tentativas para la evaluación y actividades clave, distribuidas a lo largo del periodo indicado.

Notas adicionales:
- Adaptar el contenido a las características del grupo de estudiantes.
- Mantener el lenguaje claro y motivador.
- Asegurarse de que el encuadre esté alineado con el plan curricular institucional.


## Juicios valorativos

Redacta juicios valorativos breves para cada uno de los cuatro niveles de desempeño (superior, alto, básico y bajo) establecidos en el Decreto 1290 de 2009 en Colombia. Estos juicios deben evaluar el logro de estudiantes en las competencias [COMPETENCIAS] y aprendizajes [APRENDIZAJES] del área de [ÁREA], en el grado [GRADO]; Los juicios deben ser claros y concisos, en un solo párrafo para cada nivel, sin numeración y enfocados en el nivel de logro de la competencia indicada.

## Plan de clase

## Aprendizaje-Socio-emocional

### Perfil Psicológico

Actua como un psicólogo nivel Ph.D. y ofrezca un feedback enriquecedor para mis estudiantes, enfocado en fortalecer sus competencias de trabajo en equipo y la proyección de su futuro profesional. Los estudiantes, próximos a graduarse de la educación media en un colegio rural de Colombia, han completado un formulario de caracterización de su perfil psicológico. El feedback debe ser positivo y motivador, destacando tanto sus fortalezas como oportunidades de mejora para impulsarlos a alcanzar su máximo potencial y a enfrentar con seguridad los desafíos futuros. Al final, incluye comentarios, prolijos en consejos y recursos, que categorizan su perfil psicológico, considerando aspectos como manejo emocional, personalidad, motivaciones, metas y proceso de toma de decisiones, además de motivación, resiliencia, habilidades sociales y liderazgo. Es IMPORTANTE que al final del feedback haya una sección denominada categorización del perfil psicológico, donde explicitamente se realiza la respectiva categorización. Firma el feedback asi: "Att.: [MODELO] AI, con la asistencia de Profesor Diego Beltrán en el prompt engineering."

## Evaluación de desempeño

### Anexo 5

Usando como base el cuadro del año pasado que proporciono como contexto, proponga para cada área de gestión y competencia, la Contribución individual, los Criterios de evaluación  y las Evidencias para cumplir con la meta de []. 

CONTEXTO [ANEXO 5]

### Anexo 2

## EVALS

### Exam multiple choices with critical thinking

You are an experienced educator tasked with creating a challenging and rigorous exam. Your goal is to generate a complex assessment that evaluates critical thinking skills. Please use the following information to create the exam:

<grade_level>{{grade_level}}</grade_level>
<subject>{{subject}}</subject>
<number_of_questions>{{number_of_questions}}</number_of_questions>
<question_type>{{question_type}}</question_type>
<exam_topic>{{exam_topic}}</exam_topic>

Follow these steps to create the exam:

1. Generate a complex, moderately long text related to the <subject> and <exam_topic>. This text should be appropriate for the specified <grade_level> and serve as the basis for the exam questions.

2. Create <number_of_questions> <question_type> based on the generated text. These questions should:
   a. Require critical thinking and analysis to answer
   b. Be challenging and rigorous
   c. Be directly related to the content of the generated text

Before providing the final exam, wrap your thought process in <exam_planning> tags. Consider the following:
- How to make the text sufficiently complex and challenging for the given grade level
- Ways to incorporate critical thinking elements into the questions
- List key concepts and potential question topics for each section
- Consider appropriate difficulty levels for each question
- The difficulty levels should increase with each question, the easiest first, the most difficult at the end.

After your thought process, present the exam in the following format:

<exam>
<text>
[Insert the generated complex text here]
</text>

<questions>
1. [First question]
2. [Second question]
...
[Continue for the specified number of questions]
</questions>

<keys>
[Include correct answers 1)a, 2)b, etc...]
</keys>
</exam>

Ensure that your exam is precisely rigorous, evaluates critical thinking effectively. Exam have to be written in Spanish. At the end of the exam you must put the keys or correct answers to each question into <keys> tag.

### Questions in QTI format
You are an expert in creating educational assessments in QTI (Question and Test Interoperability) format. Your task is to convert user-provided questions into well-structured QTI format XML.

Here is the user input, which may contain one or multiple questions:

<user_input>
{{user_input}}
</user_input>

Please follow these steps to create the QTI format question(s):

1. Analyze the user input to understand the question content.
2. For each question in the input:
   a. Identify the question type (e.g., multiple choice, short answer, etc.)
   b. Extract key components (stem, options if applicable, correct answer)
   c. Plan the QTI structure based on the question type
   d. Consider appropriate metadata (e.g., difficulty level, topic)
   e. Generate the QTI format XML

Before providing the final output, break down each question inside <question_breakdown> tags. In your breakdown:
1. Write out the full question text
2. Identify the question type
3. List each answer option (if applicable)
4. Note the correct answer
5. Determine the difficulty level
6. Identify the topic or subject area
7. List the main XML elements needed for this specific question type
8. Consider any potential challenges or special considerations for converting this particular question to QTI format

After your breakdown, provide the QTI format XML for each question. The output for each question should follow this structure:

<?xml version="1.0" encoding="UTF-8"?>
<assessmentItem xmlns="http://www.imsglobal.org/xsd/imsqti_v2p1" identifier="q[number]" title="[Question Title]" adaptive="false" timeDependent="false">
    <responseDeclaration identifier="RESPONSE" cardinality="single" baseType="identifier">
        <correctResponse>
            <value>[Correct response identifier]</value>
        </correctResponse>
    </responseDeclaration>
    <itemBody>
        <p>
            <question_content>[Question text goes here]</question_content>
        </p>
        [Response options if applicable]
    </itemBody>
    <outcomeDeclaration identifier="SCORE" cardinality="single" baseType="float">
        <defaultValue>
            <value>0</value>
        </defaultValue>
    </outcomeDeclaration>
</assessmentItem>

Please ensure that you:
1. Replace "[number]" with a sequential number for each question.
2. Replace "[Question Title]" with an appropriate title based on the question content.
3. Insert the question content from the <question_content> variable into the appropriate place.
4. Add appropriate <responseDeclaration> and response options based on the question type and correct answer.
5. Include any necessary metadata as attributes in the <assessmentItem> tag.

If there are multiple questions in the input, provide the breakdown and QTI output for each question separately.

Begin your response with your question breakdown wrapped in <question_breakdown> tags for the first (or only) question, followed by the complete QTI format XML output.

### QTI (deprecated)
You are an expert in creating educational assessments in QTI (Question and Test Interoperability) format. Your task is to take the provided user input and generate a well-structured QTI format question.

Here is the user input:
<user_input>
{{user_input}}
</user_input>

Please follow these steps to create the QTI format question:

1. Analyze the user input to understand the question content.
2. Generate the appropriate QTI format XML structure.
3. Insert the question content into the XML structure.

Before providing the final output, please wrap your thought process and planning in <analysis> tags. In your analysis:
1. Identify the question type (e.g., multiple choice, short answer, etc.)
2. Extract key components of the question (stem, options if applicable, correct answer)
3. Plan the QTI structure based on the question type
4. Consider appropriate metadata for the question (e.g., difficulty level, topic)
5. Ensure all necessary components are present for the QTI format

The final output should be in the following QTI format:

<assessmentItem xmlns="http://www.imsglobal.org/xsd/imsqti_v2p1" identifier="q1" title="[Question Title]" adaptive="false" timeDependent="false">
    <itemBody>
        <p>
            <question_content>{{question_content}}</question_content>
        </p>
    </itemBody>
    <responseDeclaration identifier="RESPONSE" cardinality="single" baseType="identifier">
        <correctResponse>
            [Correct response information]
        </correctResponse>
    </responseDeclaration>
</assessmentItem>

Please ensure that you:
1. Replace "[Question Title]" with an appropriate title based on the question content.
2. Insert the question content from the <question_content> variable into the <p> tag.
3. Add appropriate <responseDeclaration> information based on the question type and correct answer.

Begin your response with your thought process wrapped in <analysis> tags, followed by the complete QTI format XML output.
