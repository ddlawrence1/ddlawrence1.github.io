<?xml version="1.0"?>
<flowgorithm fileversion="4.2">
    <attributes>
        <attribute name="name" value="GuessGaming"/>
        <attribute name="authors" value="lawre"/>
        <attribute name="about" value=""/>
        <attribute name="saved" value="2024-09-29 01:53:09 PM"/>
        <attribute name="created" value="bGF3cmU7REVTS1RPUC00OUFUUkVFOzIwMjQtMDktMjk7MDE6MjY6MjQgUE07Mjg4Nw=="/>
        <attribute name="edited" value="bGF3cmU7REVTS1RPUC00OUFUUkVFOzIwMjQtMDktMjk7MDE6NTM6MDkgUE07MTsyOTk4"/>
    </attributes>
    <function name="Main" type="None" variable="">
        <parameters/>
        <body>
            <declare name="SecretNumber" type="Integer" array="False" size=""/>
            <declare name="UserGuess" type="Integer" array="False" size=""/>
            <declare name="MAX" type="Integer" array="False" size=""/>
            <assign variable="MAX" expression="8"/>
            <assign variable="SecretNumber" expression="Random(MAX)"/>
            <output expression="&quot;Please enter a number between 0 and &quot; &amp; MAX - 1" newline="True"/>
            <input variable="UserGuess"/>
            <while expression="UserGuess &lt;&gt; SecretNumber">
                <if expression="UserGuess &lt; SecretNumber">
                    <then>
                        <output expression="&quot;Too Low&quot;" newline="True"/>
                    </then>
                    <else>
                        <if expression="UserGuess &gt; SecretNumber">
                            <then>
                                <output expression="&quot;Too High&quot;" newline="True"/>
                            </then>
                            <else/>
                        </if>
                    </else>
                </if>
                <output expression="&quot;Please enter a number between 0 and 7&quot;" newline="True"/>
                <input variable="UserGuess"/>
            </while>
            <output expression="&quot;You are Correct!&quot;" newline="True"/>
        </body>
    </function>
</flowgorithm>
