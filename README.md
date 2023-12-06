# Full Prompting Examples
## Example 1: Zero-Shot Prompting
### Prompt:
Translate the word "Natural Sceince" to German  
### Response:
The correct translation of "Natural Science" into German is "Naturwissenschaft."

## Example 2: Few-Shot Prompting
### Prompt:
 Q: France
 
 A: Paris
 
 Q: England
 
 A: London
 
 Q: Iraq
 
 A: 
### Response:
Baghdad

## Example 3: Chain-of-Thought Prompting
### Prompt:
Jack has 2 pencils and he bought 3 boxes of pencils, each box is filled with 10 pencils except for one which is filled with half. How many pencils does Jack have?

### Response:
Jack initially has 2 pencils. He buys 3 boxes of pencils, each containing 10 pencils, except for one box, which is filled with half (5 pencils).

So, Jack has:
2 initial pencils + (3 boxes * 10 pencils/box) + 5 pencils from the box with half = 2 + 30 + 5 = 37 pencils.

### Prompt:
Q: I have 3 balls and then I bought two boxes each containing 4 balls but one of them contains half. How many balls do I have?

A:

3 balls I had before  

4 balls from the first box 

2 balls from the other box because it contains half 

3 + 4 + 2 = 9

Q: Hange has 4 emeralds and then she found 4 bags of emeralds, each contains 2 emeralds but one of them contains half. How many emeralds does Hange have?

A:

4 emeralds she had

2 emeralds from the first bag

2 emeralds from the second bag

2 emeralds from the third bag

1 emerald from the last bag, because it contains half

4 + 2 + 2 + 2 + 1 = 11

Q: Jack has 2 pencils and then he bought 3 boxes of pencils, two of them contain 10 pencils and one of them contains half. How many pencils does Jack have?

A:

### Response:
2 pencils Jack had initially

10 pencils in the first box

10 pencils in the second box

5 pencils in the third box, because it contains half

So, Jack has a total of 2 + 10 + 10 + 5 = 27 pencils.

## Example 4: Self-Consistency Prompting
### Prompt:
When I was 6 my sister was half my age. Now I’m 70 how old is my sister?

### Response:
When you were 6 years old, your sister was half your age, which means she was 3 years old at that time (6 / 2 = 3). The age difference between you and your sister is 3 years. Now that you are 70, you can find your sister's current age by adding the age difference to your current age:

70 + 3 = 73

So, your sister is 73 years old now.

### Prompt:
Q: There are 15 trees in the grove. Grove workers will plant trees in the grove today. After they are done,
there will be 21 trees. How many trees did the grove workers plant today?

A: We start with 15 trees. Later we have 21 trees. The difference must be the number of trees they planted.
So, they must have planted 21 - 15 = 6 trees. The answer is 6.

Q: If there are 3 cars in the parking lot and 2 more cars arrive, how many cars are in the parking lot?

A: There are 3 cars in the parking lot already. 2 more arrive. Now there are 3 + 2 = 5 cars. The answer is 5.

Q: Leah had 32 chocolates and her sister had 42. If they ate 35, how many pieces do they have left in total?

A: Leah had 32 chocolates and Leah’s sister had 42. That means there were originally 32 + 42 = 74
chocolates. 35 have been eaten. So in total they still have 74 - 35 = 39 chocolates. The answer is 39.

Q: Jason had 20 lollipops. He gave Denny some lollipops. Now Jason has 12 lollipops. How many lollipops
did Jason give to Denny?

A: Jason had 20 lollipops. Since he only has 12 now, he must have given the rest to Denny. The number of
lollipops he has given to Denny must have been 20 - 12 = 8 lollipops. The answer is 8.

Q: Shawn has five toys. For Christmas, he got two toys each from his mom and dad. How many toys does
he have now?

A: He has 5 toys. He got 2 from mom, so after that he has 5 + 2 = 7 toys. Then he got 2 more from dad, so
in total he has 7 + 2 = 9 toys. The answer is 9.

Q: There were nine computers in the server room. Five more computers were installed each day, from
monday to thursday. How many computers are now in the server room?

A: There are 4 days from monday to thursday. 5 computers were added each day. That means in total 4 * 5 =
20 computers were added. There were 9 computers in the beginning, so now there are 9 + 20 = 29 computers.
The answer is 29.

Q: Michael had 58 golf balls. On tuesday, he lost 23 golf balls. On wednesday, he lost 2 more. How many
golf balls did he have at the end of wednesday?

A: Michael initially had 58 balls. He lost 23 on Tuesday, so after that he has 58 - 23 = 35 balls. On
Wednesday he lost 2 more so now he has 35 - 2 = 33 balls. The answer is 33.

Q: Olivia has $23. She bought five bagels for $3 each. How much money does she have left?

A: She bought 5 bagels for $3 each. This means she spent $15. She has $8 left.

Q: When I was 6 my sister was half my age. Now I’m 70 how old is my sister?

A:

### Response:
As mentioned in a previous response, when you were 6 years old, your sister was half your age, which means she was 3 years old at that time. The age difference between you and your sister is 3 years. Now that you are 70, your sister would be 70 - 3 = 67 years old. So, your sister is 67 years old now.

## Example 5: Clarity of Context
Prompt:
Write a code in C# demonstrating a loop
Response:
Certainly! Here's a simple example of a for loop in C# that prints numbers from 1 to 5:

```
using System;
class Program
{
    static void Main()
    {
        // Using a for loop to iterate from 1 to 5
        for (int i = 1; i <= 5; i++)
        {
            Console.WriteLine("Number: " + i);
        }
    }
}
```

This program declares a for loop with the initialization statement int i = 1, the condition i <= 5, and the iteration statement i++ (which increments i by 1 in each iteration). Inside the loop, it prints the current value of i. The loop will run five times, printing numbers 1 through 5.

### Prompt:
I'm an amateur, I've just started to learn programming. Write 5 examples of C# code demonstrating a loop, starting with a simple one to a complex one, with elaboration of each.

### Response:
Certainly! I'll provide you with five examples of C# code demonstrating loops, progressing from simpler to more complex.

1.	Simple while loop:

```
using System;
class Program
{
    static void Main()
    {
        int count = 1;

        // Simple while loop to print numbers from 1 to 5
        while (count <= 5)
        {
            Console.WriteLine("Number: " + count);
            count++;
        }
    }
}
```

Explanation: This example uses a while loop to print numbers from 1 to 5. The loop continues executing as long as the count variable is less than or equal to 5. Inside the loop, the current value of count is printed, and count is incremented in each iteration.

2.	‘do-while’ loop:

```
using System;
class Program
{
    static void Main()
    {
        int count = 1;

        // do-while loop to print numbers from 1 to 5
        do
        {
            Console.WriteLine("Number: " + count);
            count++;
        } while (count <= 5);
    }
}
```

Explanation: Similar to the while loop, the do-while loop prints numbers from 1 to 5. The primary difference is that a do-while loop guarantees at least one execution of the loop body before checking the condition.

3.	‘for loop’ with step:

```
using System;
class Program
{
    static void Main()
    {
        // for loop to print even numbers from 2 to 10
        for (int i = 2; i <= 10; i += 2)
        {
            Console.WriteLine("Even Number: " + i);
        }
    }
}
```

Explanation: This for loop prints even numbers from 2 to 10. The loop initializes i to 2, runs as long as i is less than or equal to 10, and increments i by 2 in each iteration.

4. Nested loops:

```
using System;
class Program
{
    static void Main()
    {
        // Nested loops to create a simple multiplication table
        for (int i = 1; i <= 5; i++)
        {
            for (int j = 1; j <= 5; j++)
            {
                Console.Write(i * j + "\t");
            }
            Console.WriteLine(); // Move to the next line after each row
        }
    }
}
```

Explanation: This example demonstrates nested loops to create a simple multiplication table. The outer loop iterates over the rows, and the inner loop iterates over the columns.

5.	Loop with ‘break’ and ‘continue’:

```
using System;
class Program
{
    static void Main()
    {
        // Loop with break and continue statements
        for (int i = 1; i <= 10; i++)
        {
            if (i % 2 == 0)
            {
                Console.WriteLine("Skipping even number: " + i);
                continue; // Skip the rest of the loop body for even numbers
            }

            Console.WriteLine("Processing odd number: " + i);

            if (i == 7)
            {
                Console.WriteLine("Found the number 7. Exiting loop.");
                break; // Exit the loop when the number 7 is encountered
            }
        }
    }
}
```

Explanation: This example uses the break statement to exit the loop when the number 7 is encountered and the continue statement to skip the loop body for even numbers. It demonstrates control flow within a loop based on certain conditions. Feel free to run these examples in a C# environment to see the output and better understand how loops work!

## Example 6: Assigning Roles 
### Prompt:
What does CIA mean?

### Response:
CIA can refer to different things depending on the context. Here are a few common meanings:

1. Central Intelligence Agency: The Central Intelligence Agency is a civilian foreign intelligence service of the federal government of the United States. It is tasked with gathering, processing, and analyzing national security information from around the world.
2. Confidentiality, Integrity, and Availability (CIA): In the context of information security, CIA represents the three core principles of information security. These principles ensure that data is kept confidential, remains unaltered (integrity), and is available when needed.
3. Culinary Institute of America: The Culinary Institute of America is a well-known culinary school in the United States, offering education and training in the field of culinary arts and hospitality management.
4. Catholic Institute of America: This can refer to various Catholic educational institutions or organizations.

If you provide more context, I can offer a more specific explanation based on the context in which "CIA" is used.

### Prompt:
You are a Computer Science professor, what does CIA mean?

### Response:
In the context of computer science and information security, CIA stands for Confidentiality, Integrity, and Availability. These three principles are fundamental to information security and guide the development and implementation of secure systems:

1. Confidentiality: This principle ensures that information is only accessible to authorized individuals or systems. It involves protecting data from unauthorized access, disclosure, or exposure.

2. Integrity: Integrity involves maintaining the accuracy and reliability of data. It ensures that information is not altered or tampered with by unauthorized parties and that data remains consistent and trustworthy.

3. Availability: Availability ensures that information and resources are accessible and usable when needed. It involves preventing disruptions to services and systems, ensuring that authorized users can access the data and services they require.

These three principles collectively form the foundation of a secure computing environment and are often referred to as the CIA triad in the field of information security.

## Example 7: Output Specification
### Prompt:
In a small town named "Morioh", lives Clara. She's a 19-year-old programmer. She lives with her father Jonas, 40 years old who works as a paleontologist in a museum. Her mother, Marta, 38 years old, works as a neurosurgeon in the hospital. Covert this text to a JSON file.

### Response:
Certainly! Here's the JSON representation of the given information:

```
{
  "town": "Morioh",
  "residents": [
    {
      "name": "Clara",
      "age": 19,
      "occupation": "programmer"
    },
    {
      "name": "Jonas",
      "age": 40,
      "occupation": "paleontologist"
    },
    {
      "name": "Marta",
      "age": 38,
      "occupation": "neurosurgeon"
    }
  ]
}
```

This JSON structure includes the town name ("Morioh") and an array of residents, where each resident has a name, age, and occupation.

## Example 8: Indicating Input Data
### Prompt:
I'm a student at a university. It is a very strict one. We should not wear colorful outfits. The course is 3 months long with 3 lectures a day. Each lecture is 2 hours long and I need to look good in every one of them. Tell me what to wear each day and what should I do between lectures. Divide your answer to sections.

### Response:
Certainly! While I can't account for personal preferences and specific dress codes, I can provide you with general advice on what to wear and what activities to engage in between lectures for a polished and professional look. Please adapt these suggestions to your university's dress code and your personal style:

Wardrobe Choices:

Day 1: Monday
- Outfit: Wear a well-fitted, neutral-colored blouse/shirt with formal trousers/skirt. Choose subtle patterns or textures for added sophistication.
- Footwear: Closed-toe shoes in a neutral color.
- Accessories: Minimal jewelry – a wristwatch and simple earrings.
- Hair: Neat and well-groomed.

Day 2: Tuesday
- Outfit: A professional dress or a blouse paired with tailored pants.
- Footwear: Comfortable yet formal shoes.
- Accessories: Add a statement piece like a watch or a subtle scarf.
- Hair: Style it in a way that is both polished and easy to manage.

Day 3: Wednesday
- Outfit: A blouse with a pencil skirt or formal dress.
- Footwear: Closed-toe heels or flats.
- Accessories: Stick to the less-is-more principle, perhaps a sleek belt.
- Hair: Consider a polished updo or a sleek ponytail.

Day 4: Thursday
- Outfit: Mix and match a blouse with well-fitted trousers or a formal jumpsuit.
- Footwear: Comfortable heels or flats.
- Accessories: Keep it subtle – a bracelet or a delicate necklace.
- Hair: Opt for loose waves or a classic bun.

Day 5: Friday
- Outfit: End the week with a sophisticated blazer paired with formal pants or a skirt.
- Footwear: Closed shoes or ankle boots.
- Accessories: Choose a classic watch or elegant earrings.
- Hair: Style it according to personal preference, keeping it polished.

Between Lectures:
1. Lunch Break:
   - Utilize this time to have a balanced meal to keep your energy levels up.
   - Consider networking with classmates or professors during lunch.
2. Study Sessions:
   - Review lecture notes or work on assignments to stay ahead.
   - Find a quiet space like the library for focused study.
3. Networking Opportunities:
   - Attend any student or department events to build connections.
   - Approach professors or classmates for discussions.
4. Physical Activity:
   - Take short walks or do light stretches to refresh your mind.
   - Consider joining a sports club or fitness class for a healthy break.
5. Mindful Breaks:
   - Practice mindfulness or meditation to relax your mind.
   - Listen to calming music or read something non-academic for a mental break.

Remember to adapt these suggestions to your university's dress code policy and your personal comfort. It's essential to project professionalism while maintaining your own style and comfort.
