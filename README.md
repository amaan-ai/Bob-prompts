# Prompt Lab

<style>
:root {
  --bg: #ffffff;
  --panel: #f4f4f4;
  --panel-border: #e0e0e0;
  --text: #161616;
  --muted: #525252;
  --link: #0f62fe;
  --link-hover: #0043ce;
  --card: #ffffff;
  --card-border: #d9d9d9;
  --shadow: 0 1px 2px rgba(0, 0, 0, 0.08);
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  color: var(--text);
  background: var(--bg);
  font-family: "IBM Plex Sans", Arial, sans-serif;
  line-height: 1.6;
}

.page-layout {
  display: flex;
  gap: 2rem;
  align-items: flex-start;
}

.sidebar {
  position: sticky;
  top: 1rem;
  width: 280px;
  min-width: 280px;
  max-height: calc(100vh - 2rem);
  overflow: auto;
  background: var(--panel);
  border: 1px solid var(--panel-border);
  border-radius: 0.5rem;
  padding: 1rem;
  box-shadow: var(--shadow);
}

.sidebar h2 {
  margin: 0 0 1rem;
  font-size: 1rem;
  font-weight: 600;
}

.sidebar nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

.sidebar nav li + li {
  margin-top: 0.5rem;
}

.sidebar nav a {
  display: block;
  color: var(--text);
  text-decoration: none;
  padding: 0.625rem 0.75rem;
  border-radius: 0.375rem;
  border: 1px solid transparent;
  transition: background 0.2s ease, border-color 0.2s ease, color 0.2s ease;
}

.sidebar nav a:hover,
.sidebar nav a:focus {
  background: #e8f0ff;
  border-color: #a6c8ff;
  color: var(--link-hover);
}

.content {
  flex: 1;
  min-width: 0;
}

.hero {
  margin-bottom: 2rem;
}

.hero h1 {
  margin-bottom: 0.5rem;
  font-size: 2rem;
  line-height: 1.2;
}

.prompt-section {
  scroll-margin-top: 1rem;
  margin-bottom: 1.5rem;
  background: var(--card);
  border: 1px solid var(--card-border);
  border-radius: 0.5rem;
  padding: 1.5rem;
  box-shadow: var(--shadow);
}

.prompt-section h2 {
  margin-top: 0;
  margin-bottom: 1rem;
  font-size: 1.25rem;
  line-height: 1.3;
}

.prompt-section pre {
  margin: 0;
  white-space: pre-wrap;
  word-break: break-word;
  overflow-wrap: anywhere;
  background: #f4f4f4;
  border: 1px solid #e0e0e0;
  border-radius: 0.375rem;
  padding: 1rem;
  color: var(--text);
  font-family: "IBM Plex Mono", "SFMono-Regular", Consolas, monospace;
  font-size: 0.95rem;
  line-height: 1.7;
}

@media (max-width: 960px) {
  .page-layout {
    flex-direction: column;
  }

  .sidebar {
    position: static;
    width: 100%;
    min-width: 0;
    max-height: none;
  }
}
</style>

<div class="page-layout">
  <aside class="sidebar">
    <h2>Prompts</h2>
    <nav>
      <ul>
        <li><a href="#prompt-1">Prompt 1</a></li>
        <li><a href="#prompt-2">Prompt 2</a></li>
        <li><a href="#prompt-3">Prompt 3</a></li>
        <li><a href="#prompt-4">Prompt 4</a></li>
        <li><a href="#prompt-5">Prompt 5</a></li>
      </ul>
    </nav>
  </aside>

  <main class="content">
    <section class="hero">
      <h1>Prompt Lab</h1>
    </section>

    <section id="prompt-1" class="prompt-section">
      <h2>Prompt 1</h2>
      <pre>What is this application about?</pre>
    </section>

    <section id="prompt-2" class="prompt-section">
      <h2>Prompt 2</h2>
      <pre>Along with Routing Rules, are there any System Classification and Additional notes?</pre>
    </section>

    <section id="prompt-3" class="prompt-section">
      <h2>Prompt 3</h2>
      <pre>I have currently deployed this on codeengine, Have cloned the repo locally,  How do I run this applicaiton locally?</pre>
    </section>

    <section id="prompt-4" class="prompt-section">
      <h2>Prompt 4</h2>
      <pre>okay I did ./start.sh, and the applicaiton started running on: http://127.0.0.1:8080 

I uploaded @/uploads/Data_Integration_Table_desen.xlsx file on browser UI and got results successfully.

Next, we got two new files: 

a. @/new-files-by-client/POC\ System\ Interaction\ B\ (\ v0.3_cleaned)\ (\ (Desensitised).xlsx 

b. @/new-files-by-client/POC\ System\ Interaction\ C\ (BLIM\ 14052026\ at\ 0928\ hours)\ (Desensitised).xlsx 



When I reload the browser and test upload these 2 new files I can see the graph. I can see that these files have additional Gateaways values in column 'Data Exchange Gateway Used', for e.g. Gateaway A, etc. Also addiotional Destination System.



May I know if my current application is coded in such a way to handle additional new data point, i.e. it it able to process and display all information & graph correctly on UI? or can be missiing any info.?</pre>
    </section>

    <section id="prompt-5" class="prompt-section">
      <h2>Prompt 5</h2>
      <pre>Can we add one more rule i.e. 'Gateaway A' only supports 'External' and 'eServices' links (present in Destination Agency column value). Update the codebase accordingly, including UI and backend</pre>
    </section>
  </main>
</div>