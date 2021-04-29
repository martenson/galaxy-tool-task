### Assignment:

Use the code in this repository to create a Galaxy tool, that will convert a given Galaxy dataset from the `.mgf` format to the `.mat` format.

The result of this assignment should at minimum include an `.xml` file with the Galaxy tool definition. You can also include a short document explaining your thinking about the asignment or describe the steps taken.

The result is most probably correct if the following Galaxy Tool test passes:

```xml
    <tests>
        <test>
            <param name="input_file" value="test.mgf"/>
            <output name="output_file" file="test.mat"/>
        </test>
    </tests>
```



#### Hints and links:

* Your best friend for Galaxy tool development is a utility called `planemo`. See the [docs](https://planemo.readthedocs.io/en/latest/readme.html).
* Moreover Planemo documentation contains [section](https://planemo.readthedocs.io/en/latest/writing_standalone.html) on writing Galaxy tools.
* The most important planemo commands for you are `planemo serve` and `planemo test`. [Full list](https://planemo.readthedocs.io/en/latest/commands.html) of commands.
* Don't miss the README.md file in this repository.
* Galaxy knows the `mgf` format, but does not understand the `mat` format. You can treat `mat` files as generic `txt` files when you need to.
* You do not need to care about cornercases or invalid inputs.
* You can check out the full [XML schema](https://docs.galaxyproject.org/en/master/dev/schema.html) of what is allowed in a Galaxy tool file.
