<template>
    <div class="home-container">
        <header class="header">
            <h1>Welcome to Home</h1>
            <p>Your Vue Application</p>
        </header>

        <main class="main-content">
            <section class="hero">
                <h2>Hello, Welcome!</h2>
                <p>This is your home page</p>
                <button @click="handleClick" class="btn">Get Started</button>
            </section>

            <section class="features">
                <div class="feature-card">
                    <h3>Feature One</h3>
                    <p>Description of feature one</p>
                </div>
                <div class="feature-card">
                    <h3>Feature Two</h3>
                    <p>Description of feature two</p>
                </div>
                <div class="feature-card">
                    <h3>Feature Three</h3>
                    <p>Description of feature three</p>
                </div>
            </section>
        </main>
    </div>
</template>

<script>
export default {
    name: 'Home',
    data() {
        return {
            message: 'Welcome'
        }
    },
    methods: {
        handleClick() {
            console.log('Button clicked')
        }
    }
}
</script>

<style scoped>
.home-container {
    width: 100%;
    min-height: 100vh;
}

.header {
    text-align: center;
    padding: 40px 20px;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
}

.main-content {
    padding: 40px 20px;
}

.hero {
    text-align: center;
    margin-bottom: 60px;
}

.hero h2 {
    font-size: 32px;
    margin-bottom: 10px;
}

.btn {
    padding: 10px 20px;
    margin-top: 20px;
    background-color: #667eea;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 16px;
}

.btn:hover {
    background-color: #764ba2;
}

.features {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 20px;
}

.feature-card {
    padding: 20px;
    border: 1px solid #ddd;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.feature-card h3 {
    margin-bottom: 10px;
}
</style>