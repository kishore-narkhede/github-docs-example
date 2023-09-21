# Writing Good Documentation

## Step 1 - Using Codeblocks

Code blocks in markdown make it *very easy* for tech people to **copy, paste and share** code.
A good __Cloud Engineer__ uses Codeblocks whenever possible.

Because it allows others to copy and paste their code to replciate or research issues.
- In order to create Codeblocks, you need to use back ticks ``` 
- Not to be confused with single quotes `

```
import java.io.BufferedReader;
import java.io.FileReader;
import java.io.IOException;

public class DisplayMarkdownFile {
    public static void main(String[] args) {
        // Provide the path to your Markdown file
        String filePath = "path/to/your/markdownfile.md";

        try {
            // Open the file
            FileReader fileReader = new FileReader(filePath);
            BufferedReader bufferedReader = new BufferedReader(fileReader);

            // Read and display each line of the Markdown file
            String line;
            while ((line = bufferedReader.readLine()) != null) {
                System.out.println(line);
            }

            // Close the file
            bufferedReader.close();
        } catch (IOException e) {
            System.err.println("Error reading the Markdown file: " + e.getMessage());
        }
    }
}
```

- When you can , you should attempt to apply syntax highlighting to your codeblocks.

```Java
import java.io.BufferedReader;
import java.io.FileReader;
import java.io.IOException;

public class DisplayMarkdownFile {
    public static void main(String[] args) {
        // Provide the path to your Markdown file
        String filePath = "path/to/your/markdownfile.md";

        try {
            // Open the file
            FileReader fileReader = new FileReader(filePath);
            BufferedReader bufferedReader = new BufferedReader(fileReader);

            // Read and display each line of the Markdown file
            String line;
            while ((line = bufferedReader.readLine()) != null) {
                System.out.println(line);
            }

            // Close the file
            bufferedReader.close();
        } catch (IOException e) {
            System.err.println("Error reading the Markdown file: " + e.getMessage());
        }
    }
}
```
<!--
![Sea Face Image](https://github.com/kishore-narkhede/github-docs-example/blob/main/assets/sea_face.jpg)
-->
<img width="200px" src="https://github.com/kishore-narkhede/github-docs-example/blob/main/assets/sea_face.jpg">

Good Cloud Engineers use code blocks for both Code and Errors that appear in the console.
> Here is an example (quote)

```bash
A NullPointerException occurred: null
```

## Step -3 Use Github flavoured Task Lists

Github extends Mardown to have a list where you can check off items. <sup>[1]</sup>
- [x] - Finsh step 1
- [ ] - Finish step 2
- [ ] - Finish step 3

## Step -4 Use emojis (optional)

:cloud:


## References
- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/) <sup>[1]</sup>
- [Basic writing and formatting syntax (Github Flavoured Markdown)](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)<sup>[2]</sup>

- [Github Flavoured Markdown emoji cheatsheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)
