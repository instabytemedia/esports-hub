# Entity Relationship Diagram - Esports Hub

> **Auto-generated** from your idea analysis
> **Entities:** 3

---

## Visual Diagram

```mermaid
erDiagram
    profiles {
        uuid id PK
        text username UK
        text display_name
        text avatar_url
        timestamptz created_at
        timestamptz updated_at
    }

    ideas {
        uuid id PK
        uuid user_id FK
        uuid id
        timestamptz created_at
        timestamptz updated_at
        uuid user_id FK
        text title
        text description
        timestamptz created_at
        timestamptz updated_at
    }

    cryptos {
        uuid id PK
        uuid user_id FK
        uuid id
        timestamptz created_at
        timestamptz updated_at
        uuid user_id FK
        text name
        text symbol
        timestamptz created_at
        timestamptz updated_at
    }

    stadiums {
        uuid id PK
        uuid user_id FK
        uuid id
        timestamptz created_at
        timestamptz updated_at
        uuid user_id FK
        text name
        text description
        timestamptz created_at
        timestamptz updated_at
    }

    %% Relationships
    profiles ||--o{ ideas : owns
    profiles ||--o{ cryptos : owns
    profiles ||--o{ stadiums : owns
    ideas ||--o{ users : "A user can submit multiple ideas"
    cryptos ||--o{ users : "A user can own multiple cryptocurrencies"
    stadiums ||--o{ users : "A user can own multiple virtual stadiums"
```

---

## Entity Details

### Idea
> A concept or proposal for a new digital collectible, prediction market, or AR-powered fantasy sports league

**Fields:**
  - `id`: uuid (required) - Primary key
  - `created_at`: datetime (required) - Creation timestamp
  - `updated_at`: datetime (required) - Last update timestamp
  - `user_id`: uuid (required) - Owner user ID
  - `title`: string (required)
  - `description`: text (required)

**Relationships:**
  - one_to_many → **User**: A user can submit multiple ideas

### Crypto
> A cryptocurrency used for transactions on the platform

**Fields:**
  - `id`: uuid (required) - Primary key
  - `created_at`: datetime (required) - Creation timestamp
  - `updated_at`: datetime (required) - Last update timestamp
  - `user_id`: uuid (required) - Owner user ID
  - `name`: string (required)
  - `symbol`: string (required)

**Relationships:**
  - one_to_many → **User**: A user can own multiple cryptocurrencies

### Stadium
> A virtual stadium where users can participate in AR-powered fantasy sports leagues

**Fields:**
  - `id`: uuid (required) - Primary key
  - `created_at`: datetime (required) - Creation timestamp
  - `updated_at`: datetime (required) - Last update timestamp
  - `user_id`: uuid (required) - Owner user ID
  - `name`: string (required)
  - `description`: text (required)

**Relationships:**
  - one_to_many → **User**: A user can own multiple virtual stadiums

---

## Notes

- All entities have standard fields: `id`, `user_id`, `created_at`, `updated_at`
- `PK` = Primary Key, `FK` = Foreign Key, `UK` = Unique Key
- Copy the Mermaid code block to visualize in any Mermaid-compatible tool
- Relationships: `||--o{` = one-to-many, `||--||` = one-to-one, `}o--o{` = many-to-many
