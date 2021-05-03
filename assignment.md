### Assignment:

Use the code in this repository to create a Galaxy tool, that will convert a given Galaxy dataset from the `.mgf` format to the `.mat` format.

The result of this assignment should at minimum include an `.xml` file with the Galaxy tool definition. You can also include a paragraph or two explaining your thinking about the asignment or describe the steps taken. We will take these notes into consideration when evaluating.

You do not have to include parameters other than what is needed for the conversion. We will evaluate by putting your tool in Galaxy and running it on the test data provided. The result is most probably correct if the following Galaxy Tool test passes:

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
* Galaxy itself implements the `mgf` format, but not the `mat` format. Set the output format to generic `txt` to work around this.
* You do not need to care about cornercases or invalid inputs.
* You can check out the full [XML schema](https://docs.galaxyproject.org/en/master/dev/schema.html) of what is allowed in a Galaxy tool file.
* If you are stuck please feel free to write an email to martin.cech@recetox.muni.cz and ask specific questions.
