<template>
    <div class="license-expired-container">
        <div class="license-expired-box">
            <div class="alert-icon">
                <i class="fas fa-exclamation-triangle"></i>
            </div>
            <h1>403</h1>
            
        </div>
    </div>
</template>

<script>
import axios from "../../axios";

export default {
    name: "LicenseExpired",
    data() {
        return {
            expiryDate: "",
            licenseKey: "",
        };
    },
    created() {
        this.getLicenseInfo();
    },
    methods: {
        async getLicenseInfo() {
            try {
                const response = await axios.get("/api/license/check");
                this.expiryDate = response.data.expiryDate;

                // You can display license key if needed
                this.licenseKey = "themeforest"; // Can be retrieved from API if needed
            } catch (error) {
                console.error("Unable to get license information:", error);
                this.expiryDate = "unknown date";
            }
        },
    },
};
</script>

<style scoped>
.license-expired-container {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    background-color: #f5f5f5;
    padding: 20px;
}

.license-expired-box {
    max-width: 600px;
    width: 100%;
    background: white;
    border-radius: 8px;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    padding: 40px;
    text-align: center;
}

.alert-icon {
    font-size: 50px;
    color: #ff5252;
    margin-bottom: 20px;
}

h1 {
    color: #333;
    margin-bottom: 20px;
    font-size: 24px;
}

p {
    color: #666;
    margin-bottom: 15px;
    font-size: 16px;
}

.contact-info {
    margin-top: 30px;
    padding: 20px;
    background-color: #f9f9f9;
    border-radius: 5px;
}

.contact-info h3 {
    margin-bottom: 15px;
    color: #333;
    font-size: 18px;
}

.contact-info i {
    margin-right: 10px;
    color: #666;
}

.license-key {
    margin-top: 30px;
    padding: 15px;
    background-color: #eef7ff;
    border-radius: 5px;
    border-left: 4px solid #3498db;
}

.license-key strong {
    color: #3498db;
}

.contact-button {
    margin-top: 30px;
}

.contact-link {
    display: inline-block;
    background-color: #25d366;
    color: white;
    padding: 12px 24px;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
    transition: background-color 0.3s;
}

.contact-link:hover {
    background-color: #128c7e;
}

.contact-link i {
    margin-right: 8px;
}
</style>
