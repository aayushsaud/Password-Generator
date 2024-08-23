<h1>Simple Password Generator</h1>

<p>This is a simple bash script that generates random passwords using the <code>openssl</code> library. The script prompts the user to enter the desired length of the password and generates five random passwords based on the input length.</p>

<h2>How to Use</h2>

<ol>
    <li>Make sure you have <code>openssl</code> installed on your system. If not, you can install it using your package manager. For example:
        <ul>
            <li>On Debian/Ubuntu: <code>sudo apt-get install openssl</code></li>
            <li>On CentOS/RedHat: <code>sudo yum install openssl</code></li>
        </ul>
    </li>
    <li>Save the script in a file, for example <code>password_generator.sh</code>.</li>
    <li>Make the script executable:
        <pre><code>chmod +x password_generator.sh</code></pre>
    </li>
    <li>Run the script:
        <pre><code>./password_generator.sh or bash password_generator.sh</code></pre>
    </li>
    <li>When prompted, enter the desired password length.</li>
    <li>The script will generate and display five random passwords of the specified length.</li>
</ol>

<h2>Example Output</h2>

<p>After running the script, you might see something like the following:</p>

<pre><code>This is a simple password generator
Please enter the length of the password: 
12
<br>
4B3hS8JGx2fP
z8F7yQiD6UjK
n0VZpQmLw2rT
fP8Hs7Dx3LqN
J4tGwQkX9RpV
</code></pre>

<h2>Notes</h2>

<ul>
    <li>The generated passwords are derived from base64-encoded random bytes. They are not guaranteed to be valid base64 strings but rather contain base64 characters.</li>
    <li>The length of the generated passwords is controlled by the user input.</li>
    <li>Be cautious with the length input; very short lengths might lead to easily guessable passwords, and extremely long lengths might not be practical.</li>
</ul>
