# 1. Next.js – API Calling in the Client Side (App Router)

To call APIs created in the App Router from a client component, use the `fetch()` method with an endpoint that starts with the `/api` folder path.

---

### Basic Syntax

```javascript
await fetch('api/ContactApi')
```

---

### Common Use Cases

####  Call a Contact API (from `src/app/api/ContactApi/route.ts`) **without parameters** on component mount

```javascript
useEffect(() =>{
const fnFetchContact = async () =>{
	const LdContact = await fetch('api/ContactApi')
	const LdResult = await LdContact.json()
	setContactValue(LdResult)
}
fnFetchContact()
},[]}
```

#### Call a Contact API **with parameters** (e.g., `email`) on component mount

```javascript
useEffect(() =>{
const fnFetchContact = async () =>{
	const LdContact = await fetch('api/ContactApi?email="xyz@email.com"')
	const LdResult = await LdContact.json()
	setContactValue(LdResult)
}
fnFetchContact()
},[]}
```