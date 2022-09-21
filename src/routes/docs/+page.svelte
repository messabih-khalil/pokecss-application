<script>
	import Code from '../../components/Code.svelte';
    import file from '../../assets/pokecss.zip'
</script>

<div>
	<p class="font-4x font-500">Get started</p>
	<!-- using cdn -->
    <p class="font-3x mgt-2 mgb-2">Methods :</p>
	<div>
		<p class="font-3x mgt-2 mgb-2 font-600">Method one : <span class="blue-900">Using cdn</span></p>
		<p class="mgb-2 blue-700"> Just copy and paste the link in the html head page </p>
		<Code
			code='
<link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/gh/messabih-khalil/Pokecss/main.css">
        '
		/>
	</div>
    <!-- download and use'it -->
    <div>
        <p class="font-3x mgt-2 mgb-2 font-600">Method Two : <span class="blue-900">Download And Use'it</span></p>
		<p class="mgb-2 blue-700 font-600"> I recommend you to use this method <span class="black font-500">because pokecss gives you flexibility and so much classes to provides in your project so that what make <span class="blue-700">pokecss library </span>a little bit bigger , but dont' worry i will show you steps to reduce and remove unused classes from the library after complete your project .</span> </p>
        <p class="font-3x mgt-2 mgb-2 purple-900 font-600">Steps :</p>
        <ul class="pdl-2">
            <li>
                > Download the library <a href="{file}" download="pokecss.zip">download</a> 
            </li>
            <li>
                > Unzip compressed folder
            </li>
            <li>
                > Copy "main.css" to your assets project
            </li>
            <p class="blue-500 font-3x font-500 mgb-2 mgt-2">After complete your project it's time to reduce main.css file and remove unused css</p>
            <li>
                <span class="font-3x font-500">
                    Vue js : 
                </span>
                <ul class="pdl-2 mgt-2 mgb-2">
            
                        <li>
                            > Visit Purge css vue documentation : <a href="https://purgecss.com/guides/vue.html">Purgecss vue</a>
                        </li>
                    
                </ul>
            </li>
            <li>
                <span class="font-3x font-500">
                    React js : 
                </span>
                <ul class="pdl-2 mgt-2 mgb-2">
            
                        <li>
                            > Visit Purge css react documentation : <a href="https://purgecss.com/guides/react.html">Purgecss react</a>
                        </li>
                    
                </ul>
            </li>
            <li>
                <span class="font-3x font-500">
                    Next js : 
                </span>
                <ul class="pdl-2 mgt-2 mgb-2">
            
                        <li>
                            > Visit Purge css next documentation : <a href="https://purgecss.com/guides/next.html">Purgecss next</a>
                        </li>
                    
                </ul>
            </li>
            <li>
                <span class="font-3x font-500">
                    Nuxt js : 
                </span>
                <ul class="pdl-2 mgt-2 mgb-2">
            
                        <li>
                            > Visit Purge css nuxt documentation : <a href="https://purgecss.com/guides/nuxt.html">Purgecss nuxt</a>
                        </li>
                    
                </ul>
            </li>
            <li>
                <span class="font-3x font-500">
                    Svelte js : 
                </span>
                <ul class="pdl-2 mgt-2 mgb-2">
            
                        <li>
                            > Purgecss documentation doesn't have guide to svelte so this is the solution : <a href="https://openbase.com/js/purgecss-from-svelte/documentation">Purgecss svelte</a>
                        </li>
                    
                </ul>
            </li>
            <li>
                <span class="font-3x font-500">
                    Without framework : 
                </span>
                <ul class="pdl-2 mgt-2 mgb-2">
            
                        <li>
                            > you need node js installed in your machine : <a href="https://nodejs.org/en/">node js</a>
                        </li>
                        <li>
                            > Open command line in your root project, copy and paste this command :
                            <ul>
                                <li>
                                    <Code code='
npm init

npm install

npm install purgecss -g

                                    '/>
                                </li>

                                <li>
                                    > After installed purgecss
                                    > You need to put the path where you copied <span class="blue-500">"main.css"</span> file and where you put html files like that : <span class="font-600">purgecss --css 'path of main.css' --content 'path of html files'  --output "where you want to output the result" , <span class="red-500">and run command .</span></span>
                                    <p class="mgt-2 mgb-2 font-3x font-500">
                                        Exemple
                                    </p>
                                    <Code code="
purgecss --css src/assets/main.css --content src/**/*.html  --output build/css/
                                    "/>
                                </li>
                            </ul>
                        </li>
                    
                </ul>
            </li>
        </ul>
    </div>
</div>
