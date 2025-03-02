# State Management with React Query

## Why React Query?

- **Efficient data fetching & caching**
- **Automatic background refetching**
- **Reduces unnecessary API calls**
- **Optimistic updates for better UX**

---

## Implementation in the App:

```javascript
import { useQuery } from "@tanstack/react-query";
import { fetchCryptoPrices } from "../utils/fetchCrypto";

const { data, isLoading, refetch } = useQuery({
  queryKey: ["cryptoPrices"],
  queryFn: fetchCryptoPrices,
  refetchInterval: 30000, // Auto refresh every 30s
});
```
